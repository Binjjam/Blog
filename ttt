const router = require('koa-router')();
const accountController = require('../controller/account');

router.get('/', async (ctx, next) => {
  await ctx.render('index', {
    title: 'Hello Koa 2!'
  })
})

router.get('/string', async (ctx, next) => {
  ctx.body = 'koa2 string'
})

router.get('/json', async (ctx, next) => {
  ctx.body = {
    title: 'koa2 json'
  }
})

router.get('/test', async (ctx, next) => {
  ctx.body = {
    isShow: "1",
    config: [
    {
    iconId: "3001",
    eventType: "SHOW_WEB",
    eventData: {
    url: "http://api.4399sy.com/mycenter/main",
    openDst: "0",
    isFullScreen: "1"
    }
    },
    {
    iconId: "2003",
    eventType: "SHOW_WEB",
    eventData: {
    url: "http://faq.4399sy.com/cs/robot/index?",
    openDst: "0",
    isFullScreen: "1"
    }
    },
    {
    iconId: "4001",
    eventType: "SHOW_CLOSE",
    eventData: {
    description: ""
    }
    },
    {
    iconId: "2003",
    eventType: "SHOW_ADS",
    eventData: {
    idKey: "",
    appKey: "",
    adType: "1",
    showDelay: "15",
    hideDelay: "8"
    }
    }
    ],
    property: {
    defaultX: "0",
    defaultY: "0.200000",
    defaultIsShowMenu: "1",
    hidenType: "2",
    hidenAlpha: "0.40"
    },
    metaData: {
    shareKey: "sh8778f02fefc52c5e",
    ocsKey: "217dc3f64c8075042ba70",
    ocsServer: "124.243.195.63",
    ocsPort: "8888"
    }
    }
})


// 登录路由
router.post('/login',accountController.login);
router.post('/account',accountController.addAccount);
router.put('/account',accountController.updateAccount);

module.exports = router
