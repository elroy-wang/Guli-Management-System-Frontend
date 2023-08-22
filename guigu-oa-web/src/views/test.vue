<template>
  <div>
    <div>账号切换</div>
    <button @click="admin()"
            type="default"
            size="mini">admin</button>
    <button @click="zhangsan()"
            type="default"
            size="mini">张三</button>
    <button @click="lisi()"
            type="default"
            size="mini">李四</button>
    <div>当前token：{{ token }}</div>
  </div>
</template>

<script>
export default {
  name: "Test",

  data () {
    return {
      token: ''
    };
  },

  created () {
    this.token = window.localStorage.getItem('token')
  },

  methods: {
    admin () {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDcyNDQ2t7Aw1VEqLU4t8kwBikGYeYm5qUAtiSm5mXlKtQDtohv2QgAAAA.YNNqMccdk7JS2u2-oZ3fKJq-2fice2JGPY89FsjhG-qZtaMNa4uBct-IQBsyo9vaTaSqpJH0_FBA6t6REi0OQA'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },
    zhangsan () {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDcyNDQ2t7Q00FEqLU4t8kxRsjKHMPMSc1OBWqoyEvPSjZVqAR40cihDAAAA.XyBpOyeSj6LHTRcYrhZC2AWIiiJFlHbQ13nONQ15rAxOqIZroSpgruqd9SfEs89c3T-aUgxsQWevh70qczUAaw'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },
    lisi () {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDcyNDQ2tzSx0FEqLU4t8kxRsjKBMPMSc1OBWnIyTZRqAdh65Q5AAAAA.OeuN86aV6eDIocOcTy_K6xJIj44hvT5bmnxD6uPnQh34KnXWcq8rX049_N5ne4GPvSeiJo40KoMgRrmsPe95wQ'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    }
  }
}
</script>
