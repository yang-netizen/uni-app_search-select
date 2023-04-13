# uni-app_search-select
input 模糊查询

使用方式
  <comboxEnhance :border="false" emptyTips="暂无数据"  :candidates="candidates"
                           placeholder="请输入并检索样品名称" v-model="checkFrom.sbmc"
                           @inputValue="handleSearchEditNew" @change="handleSelectEditNew"></comboxEnhance>
