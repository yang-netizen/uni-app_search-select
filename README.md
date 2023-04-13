# uni-app_search-select
input 模糊查询

使用方式
  <comboxEnhance :border="false" emptyTips="暂无数据"  :candidates="candidates"
                           placeholder="请输入并检索样品名称" v-model="checkFrom.sbmc"
                           @inputValue="handleSearchEditNew" @change="handleSelectEditNew"></comboxEnhance>
  数据结构不一样时                   
 candidates(){
                // 对象数组时，可以用计算属性转换成字符串数组。字符串数组时，不需要。
                return (this.ypmcInfoList||[]).map(v=>v.sbmc);
            }
