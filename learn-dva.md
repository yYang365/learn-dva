# dva

参考：

https://github.com/dvajs/dva/blob/master/README_zh-CN.md

# dva

[![NPM version](https://img.shields.io/npm/v/dva.svg?style=flat)](https://npmjs.org/package/dva)
[![Build Status](https://img.shields.io/travis/dvajs/dva.svg?style=flat)](https://travis-ci.org/dvajs/dva)
[![Coverage Status](https://img.shields.io/coveralls/dvajs/dva.svg?style=flat)](https://coveralls.io/r/dvajs/dva)
[![NPM downloads](http://img.shields.io/npm/dm/dva.svg?style=flat)](https://npmjs.org/package/dva)
[![Dependencies](https://david-dm.org/dvajs/dva/status.svg)](https://david-dm.org/dvajs/dva)
[![Join the chat at https://gitter.im/dvajs/Lobby](https://img.shields.io/gitter/room/dvajs/Lobby.svg?style=flat)](https://gitter.im/dvajs/Lobby?utm_source=share-link&utm_medium=link&utm_campaign=share-link)

[View README in English](README.md)

基于 [redux](https://github.com/reactjs/redux)、[redux-saga](https://github.com/redux-saga/redux-saga) 和 [react-router](https://github.com/ReactTraining/react-router) 的轻量级前端框架。(Inspired by [elm](http://elm-lang.org/) and [choo](https://github.com/yoshuawuyts/choo))

---

## 特性

* **易学易用**：仅有 6 个 api，对 redux 用户尤其友好
* **elm 概念**：通过 `reducers`, `effects` 和 `subscriptions` 组织 model
* **支持 mobile 和 react-native**：跨平台 ([react-native 例子](https://github.com/sorrycc/dva-example-react-native))
* **支持 HMR**：目前基于 [babel-plugin-dva-hmr](https://github.com/dvajs/babel-plugin-dva-hmr) 支持 components、routes 和 models 的 HMR
* **动态加载 Model 和路由**：按需加载加快访问速度 ([例子](https://github.com/dvajs/dva/blob/master/docs/API_zh-CN.md#dvadynamic))
* **插件机制**：比如 [dva-loading](https://github.com/dvajs/dva/tree/master/packages/dva-loading) 可以自动处理 loading 状态，不用一遍遍地写 showLoading 和 hideLoading
* **完善的语法分析库 [dva-ast](https://github.com/dvajs/dva-ast)**：[dva-cli](https://github.com/dvajs/dva-cli) 基于此实现了智能创建 model, router 等
* **支持 TypeScript**：通过 d.ts ([例子](https://github.com/sorrycc/dva-boilerplate-typescript))

## 为什么用 dva ?

* [Why dva and what's dva](https://github.com/dvajs/dva/issues/1)
* [支付宝前端应用架构的发展和选择](https://www.github.com/sorrycc/blog/issues/6)

## Demos

* [Count](https://stackblitz.com/edit/dva-example-count): 简单计数器
* [User Dashboard](https://github.com/dvajs/dva/tree/master/packages/dva-example-user-dashboard): 用户管理
* [HackerNews](https://github.com/dvajs/dva-hackernews):  ([Demo](https://dvajs.github.io/dva-hackernews/))，HackerNews Clone
* [antd-admin](https://github.com/zuiidea/antd-admin): ([Demo](http://antd-admin.zuiidea.com/))，基于 antd 和 dva 的后台管理应用
* [github-stars](https://github.com/sorrycc/github-stars): ([Demo](http://sorrycc.github.io/github-stars/#/?_k=rmj86f))，Github Star 管理应用
* [react-native-dva-starter](https://github.com/nihgwu/react-native-dva-starter): 集成了 dva 和 react-navigation 典型应用场景的 React Native 实例
* [dva-example-nextjs](https://github.com/dvajs/dva/tree/master/packages/dva-example-nextjs): 和 next.js 整合使用
* [Account System](https://github.com/yvanwangl/AccountSystem.git): 小型库存管理系统

## 快速上手

[12 步 30 分钟，完成用户管理的 CRUD 应用 (react+dva+antd)](https://github.com/sorrycc/blog/issues/18)

## FAQ

### 命名由来？

> D.Va拥有一部强大的机甲，它具有两台全自动的近距离聚变机炮、可以使机甲飞跃敌人或障碍物的推进器、 还有可以抵御来自正面的远程攻击的防御矩阵。

—— 来自 [守望先锋](http://ow.blizzard.cn/heroes/dva) 。

<img src="https://zos.alipayobjects.com/rmsportal/psagSCVHOKQVqqNjjMdf.jpg" width="200" height="200" />

### 是否可用于生产环境？

当然！公司内用于生产环境的项目估计已经有 200+ 。

### 是否支持 IE8 ？

不支持。

## 下一步

以下能帮你更好地理解和使用 dva ：

* 理解 dva 的 [8 个概念](https://github.com/dvajs/dva/blob/master/docs/Concepts_zh-CN.md) ，以及他们是如何串起来的
* 掌握 dva 的[所有 API](https://github.com/dvajs/dva/blob/master/docs/API_zh-CN.md)
* 查看 [dva 知识地图](https://github.com/dvajs/dva-knowledgemap) ，包含 ES6, React, dva 等所有基础知识
* 查看 [更多 FAQ](https://github.com/dvajs/dva/issues?q=is%3Aissue+is%3Aclosed+label%3Afaq)，看看别人通常会遇到什么问题
* 如果你基于 dva-cli 创建项目，最好了解他的 [配置方式](https://github.com/sorrycc/roadhog#配置)


还要了解更多?

* 看看 dva 的前身 [React + Redux 最佳实践](https://github.com/sorrycc/blog/issues/1)，知道 dva 是怎么来的
* 在 gitc 分享 dva 的 PPT ：[React 应用框架在蚂蚁金服的实践](http://slides.com/sorrycc/dva)
* 如果还在用 dva@1.x，请尽快 [升级到 2.x](https://github.com/sorrycc/blog/issues/48)

## 社区

> 之前在 dvaantdpro 1、2 群的请勿重复加入。

<img src="https://gw.alipayobjects.com/zos/rmsportal/WdeuPFPzlKkfEWtxxeGL.jpg" width="200" />

扫码加微信群。(群满 100 人后，可加 `sorryccpro` 备注 `dva` 邀请加入）

## License

[MIT](https://tldrlegal.com/license/mit-license)

># 理解 dva 的 8 个概念 ，以及他们是如何串起来的

# Concepts

[View this in English](./Concepts.md)

## 数据流向

数据的改变发生通常是通过用户交互行为或者浏览器行为（如路由跳转等）触发的，当此类行为会改变数据的时候可以通过 `dispatch` 发起一个 action，如果是同步行为会直接通过 `Reducers` 改变 `State` ，如果是异步行为（副作用）会先触发 `Effects` 然后流向 `Reducers` 最终改变 `State`，所以在 dva 中，数据流向非常清晰简明，并且思路基本跟开源社区保持一致（也是来自于开源社区）。

<img src="https://zos.alipayobjects.com/rmsportal/PPrerEAKbIoDZYr.png" width="807" />

## Models

### State

`type State = any`

State 表示 Model 的状态数据，通常表现为一个 javascript 对象（当然它可以是任何值）；操作的时候每次都要当作不可变数据（immutable data）来对待，保证每次都是全新对象，没有引用关系，这样才能保证 State 的独立性，便于测试和追踪变化。

在 dva 中你可以通过 dva 的实例属性 `_store` 看到顶部的 state 数据，但是通常你很少会用到:

```javascript
const app = dva();
console.log(app._store); // 顶部的 state 数据
```

### Action

`type AsyncAction = any`

Action 是一个普通 javascript 对象，它是改变 State 的唯一途径。无论是从 UI 事件、网络回调，还是 WebSocket 等数据源所获得的数据，最终都会通过 dispatch 函数调用一个 action，从而改变对应的数据。action 必须带有 `type` 属性指明具体的行为，其它字段可以自定义，如果要发起一个 action 需要使用 `dispatch` 函数；需要注意的是 `dispatch` 是在组件 connect Models以后，通过 props 传入的。
```
dispatch({
  type: 'add',
});
```

### dispatch 函数

`type dispatch = (a: Action) => Action`

dispatching function 是一个用于触发 action 的函数，action 是改变 State 的唯一途径，但是它只描述了一个行为，而 dipatch 可以看作是触发这个行为的方式，而 Reducer 则是描述如何改变数据的。

在 dva 中，connect Model 的组件通过 props 可以访问到 dispatch，可以调用 Model 中的 Reducer 或者 Effects，常见的形式如：

```javascript
dispatch({
  type: 'user/add', // 如果在 model 外调用，需要添加 namespace
  payload: {}, // 需要传递的信息
});
```

### Reducer

`type Reducer<S, A> = (state: S, action: A) => S`

Reducer（也称为 reducing function）函数接受两个参数：之前已经累积运算的结果和当前要被累积的值，返回的是一个新的累积结果。该函数把一个集合归并成一个单值。

Reducer 的概念来自于是函数式编程，很多语言中都有 reduce API。如在 javascript 中：

```javascript
[{x:1},{y:2},{z:3}].reduce(function(prev, next){
    return Object.assign(prev, next);
})
//return {x:1, y:2, z:3}
```

在 dva 中，reducers 聚合积累的结果是当前 model 的 state 对象。通过 actions 中传入的值，与当前 reducers 中的值进行运算获得新的值（也就是新的 state）。需要注意的是 Reducer 必须是[纯函数](https://github.com/MostlyAdequate/mostly-adequate-guide/blob/master/ch3.md)，所以同样的输入必然得到同样的输出，它们不应该产生任何副作用。并且，每一次的计算都应该使用[immutable data](https://github.com/MostlyAdequate/mostly-adequate-guide/blob/master/ch3.md#reasonable)，这种特性简单理解就是每次操作都是返回一个全新的数据（独立，纯净），所以热重载和时间旅行这些功能才能够使用。

### Effect

Effect 被称为副作用，在我们的应用中，最常见的就是异步操作。它来自于函数编程的概念，之所以叫副作用是因为它使得我们的函数变得不纯，同样的输入不一定获得同样的输出。

dva 为了控制副作用的操作，底层引入了[redux-sagas](http://superraytin.github.io/redux-saga-in-chinese)做异步流程控制，由于采用了[generator的相关概念](http://www.ruanyifeng.com/blog/2015/04/generator.html)，所以将异步转成同步写法，从而将effects转为纯函数。至于为什么我们这么纠结于 __纯函数__，如果你想了解更多可以阅读[Mostly adequate guide to FP](https://github.com/MostlyAdequate/mostly-adequate-guide)，或者它的中文译本[JS函数式编程指南](https://www.gitbook.com/book/llh911001/mostly-adequate-guide-chinese/details)。

### Subscription

Subscriptions 是一种从 __源__ 获取数据的方法，它来自于 elm。

Subscription 语义是订阅，用于订阅一个数据源，然后根据条件 dispatch 需要的 action。数据源可以是当前的时间、服务器的 websocket 连接、keyboard 输入、geolocation 变化、history 路由变化等等。

```javascript
import key from 'keymaster';
...
app.model({
  namespace: 'count',
  subscriptions: {
    keyEvent(dispatch) {
      key('⌘+up, ctrl+up', () => { dispatch({type:'add'}) });
    },
  }
});
```

## Router

这里的路由通常指的是前端路由，由于我们的应用现在通常是单页应用，所以需要前端代码来控制路由逻辑，通过浏览器提供的 [History API](http://mdn.beonex.com/en/DOM/window.history.html) 可以监听浏览器url的变化，从而控制路由相关操作。

dva 实例提供了 router 方法来控制路由，使用的是[react-router](https://github.com/reactjs/react-router)。

```javascript
import { Router, Route } from 'dva/router';
app.router(({history}) =>
  <Router history={history}>
    <Route path="/" component={HomePage} />
  </Router>
);
```

## Route Components

在[组件设计方法](https://github.com/dvajs/dva-docs/blob/master/v1/zh-cn/tutorial/04-%E7%BB%84%E4%BB%B6%E8%AE%BE%E8%AE%A1%E6%96%B9%E6%B3%95.md)中，我们提到过 Container Components，在 dva 中我们通常将其约束为 Route Components，因为在 dva 中我们通常以页面维度来设计 Container Components。

所以在 dva 中，通常需要 connect Model的组件都是 Route Components，组织在`/routes/`目录下，而`/components/`目录下则是纯组件（Presentational Components）。

## 参考引申

- [redux docs](http://redux.js.org/docs/Glossary.html)
- [redux docs 中文](http://cn.redux.js.org/index.html)
- [Mostly adequate guide to FP](https://github.com/MostlyAdequate/mostly-adequate-guide)
- [JS函数式编程指南](https://www.gitbook.com/book/llh911001/mostly-adequate-guide-chinese/details)
- [choo docs](https://github.com/yoshuawuyts/choo)
- [elm](http://elm-lang.org/blog/farewell-to-frp)



# API

[View this in English](./API.md)

## 输出文件
### dva

默认输出文件。

### dva/router

默认输出 [react-router](https://github.com/ReactTraining/react-router) 接口， [react-router-redux](https://github.com/reactjs/react-router-redux) 的接口通过属性 routerRedux 输出。

比如：

```js
import { Router, Route, routerRedux } from 'dva/router';
```

### dva/fetch

异步请求库，输出 [isomorphic-fetch](https://github.com/matthew-andrews/isomorphic-fetch) 的接口。不和 dva 强绑定，可以选择任意的请求库。

### dva/saga

输出 [redux-saga](https://github.com/yelouafi/redux-saga) 的接口，主要用于用例的编写。（用例中需要用到 effects）

### dva/dynamic

解决组件动态加载问题的 util 方法。

比如：

```js
import dynamic from 'dva/dynamic';

const UserPageComponent = dynamic({
  app,
  models: () => [
    import('./models/users'),
  ],
  component: () => import('./routes/UserPage'),
});
```

`opts` 包含：

* app: dva 实例，加载 models 时需要
* models: 返回 Promise 数组的函数，Promise 返回 dva model
* component：返回 Promise 的函数，Promise 返回 React Component

## dva API
### `app = dva(opts)`

创建应用，返回 dva 实例。(注：dva 支持多实例)

`opts` 包含：

* `history`：指定给路由用的 history，默认是 `hashHistory`
* `initialState`：指定初始数据，优先级高于 model 中的 state，默认是 `{}`

如果要配置 history 为 `browserHistory`，可以这样：

```js
import createHistory from 'history/createBrowserHistory';
const app = dva({
  history: createHistory(),
});
```

另外，出于易用性的考虑，`opts` 里也可以配所有的 [hooks](#appusehooks) ，下面包含全部的可配属性：

```js
const app = dva({
  history,
  initialState,
  onError,
  onAction,
  onStateChange,
  onReducer,
  onEffect,
  onHmr,
  extraReducers,
  extraEnhancers,
});
```

### `app.use(hooks)`

配置 hooks 或者注册插件。（插件最终返回的是 hooks ）

比如注册 [dva-loading](https://github.com/dvajs/dva-loading) 插件的例子：

```js
import createLoading from 'dva-loading';
...
app.use(createLoading(opts));
```

`hooks` 包含：

#### `onError((err, dispatch) => {})`

`effect` 执行错误或 `subscription` 通过 `done` 主动抛错时触发，可用于管理全局出错状态。

注意：`subscription` 并没有加 `try...catch`，所以有错误时需通过第二个参数 `done` 主动抛错。例子：

```js
app.model({
  subscriptions: {
    setup({ dispatch }, done) {
      done(e);
    },
  },
});
```

如果我们用 antd，那么最简单的全局错误处理通常会这么做：

```js
import { message } from 'antd';
const app = dva({
  onError(e) {
    message.error(e.message, /* duration */3);
  },
});
```

#### `onAction(fn | fn[])`

在 action 被 dispatch 时触发，用于注册 redux 中间件。支持函数或函数数组格式。

例如我们要通过 [redux-logger](https://github.com/evgenyrodionov/redux-logger) 打印日志：

```js
import createLogger from 'redux-logger';
const app = dva({
  onAction: createLogger(opts),
});
```

#### `onStateChange(fn)`

`state` 改变时触发，可用于同步 `state` 到 localStorage，服务器端等。

#### `onReducer(fn)`

封装 reducer 执行。比如借助 [redux-undo](https://github.com/omnidan/redux-undo) 实现 redo/undo ：

```js
import undoable from 'redux-undo';
const app = dva({
  onReducer: reducer => {
    return (state, action) => {
      const undoOpts = {};
      const newState = undoable(reducer, undoOpts)(state, action);
      // 由于 dva 同步了 routing 数据，所以需要把这部分还原
      return { ...newState, routing: newState.present.routing };
    },
  },
});
```

#### `onEffect(fn)`

封装 effect 执行。比如 [dva-loading](https://github.com/dvajs/dva-loading) 基于此实现了自动处理 loading 状态。

#### `onHmr(fn)`

热替换相关，目前用于 [babel-plugin-dva-hmr](https://github.com/dvajs/babel-plugin-dva-hmr) 。

#### `extraReducers`

指定额外的 reducer，比如 [redux-form](https://github.com/erikras/redux-form) 需要指定额外的 `form` reducer：

```js
import { reducer as formReducer } from 'redux-form'
const app = dva({
  extraReducers: {
    form: formReducer,
  },
});
```

#### `extraEnhancers`

指定额外的 [StoreEnhancer](https://github.com/reactjs/redux/blob/master/docs/Glossary.md#store-enhancer) ，比如结合 [redux-persist](https://github.com/rt2zz/redux-persist) 的使用：

```js
import { persistStore, autoRehydrate } from 'redux-persist';
const app = dva({
  extraEnhancers: [autoRehydrate()],
});
persistStore(app._store);
```

### `app.model(model)`

注册 model，详见  [#Model](#model)  部分。

### `app.unmodel(namespace)`

取消 model 注册，清理 reducers, effects 和 subscriptions。subscription 如果没有返回 unlisten 函数，使用 `app.unmodel` 会给予警告⚠️。

### `app.router(({ history, app }) => RouterConfig)`

注册路由表。

通常是这样的：

```js
import { Router, Route } from 'dva/router';
app.router(({ history }) => {
  return (
    <Router history={history}>
      <Route path="/" component={App} />
    <Router>
  );
});
```

推荐把路由信息抽成一个单独的文件，这样结合 [babel-plugin-dva-hmr](https://github.com/dvajs/babel-plugin-dva-hmr) 可实现路由和组件的热加载，比如：

```js
app.router(require('./router'));
```

而有些场景可能不使用路由，比如多页应用，所以也可以传入返回 JSX 元素的函数。比如：

```js
app.router(() => <App />);
```

### `app.start(selector?)`

启动应用。`selector` 可选，如果没有 `selector` 参数，会返回一个返回 JSX 元素的函数。

```js
app.start('#root');
```

那么什么时候不加 `selector`？常见场景有测试、node 端、react-native 和 i18n 国际化支持。

比如通过 react-intl 支持国际化的例子：

```js
import { IntlProvider } from 'react-intl';
...
const App = app.start();
ReactDOM.render(<IntlProvider><App /></IntlProvider>, htmlElement);
```

## Model
model 是 dva 中最重要的概念。以下是典型的例子：

```js
app.model({
  namespace: 'todo',
  state: [],
  reducers: {
    add(state, { payload: todo }) {
      // 保存数据到 state
      return [...state, todo];
    },
  },
  effects: {
    *save({ payload: todo }, { put, call }) {
      // 调用 saveTodoToServer，成功后触发 `add` action 保存到 state
      yield call(saveTodoToServer, todo);
      yield put({ type: 'add', payload: todo });
    },
  },
  subscriptions: {
    setup({ history, dispatch }) {
      // 监听 history 变化，当进入 `/` 时触发 `load` action
      return history.listen(({ pathname }) => {
        if (pathname === '/') {
          dispatch({ type: 'load' });
        }
      });
    },
  },
});
```

model 包含 5 个属性：

### namespace

model 的命名空间，同时也是他在全局 state 上的属性，只能用字符串，不支持通过 `.` 的方式创建多层命名空间。

### state

初始值，优先级低于传给 `dva()` 的 `opts.initialState`。

比如：

```
const app = dva({
  initialState: { count: 1 },
});
app.model({
  namespace: 'count',
  state: 0,
});
```

此时，在 `app.start()` 后 state.count 为 1 。

### reducers

以 key/value 格式定义 reducer。用于处理同步操作，唯一可以修改 `state` 的地方。由 `action` 触发。

格式为 `(state, action) => newState` 或 `[(state, action) => newState, enhancer]`。

详见： https://github.com/dvajs/dva/blob/master/packages/dva-core/test/reducers.test.js

### effects

以 key/value 格式定义 effect。用于处理异步操作和业务逻辑，不直接修改 `state`。由 `action` 触发，可以触发 `action`，可以和服务器交互，可以获取全局 `state` 的数据等等。

格式为 `*(action, effects) => void` 或 `[*(action, effects) => void, { type }]`。

type 类型有：

* `takeEvery`
* `takeLatest`
* `throttle`
* `watcher`

详见：https://github.com/dvajs/dva/blob/master/packages/dva-core/test/effects.test.js

### subscriptions

以 key/value 格式定义 subscription。subscription 是订阅，用于订阅一个数据源，然后根据需要 dispatch 相应的 action。在 `app.start()` 时被执行，数据源可以是当前的时间、服务器的 websocket 连接、keyboard 输入、geolocation 变化、history 路由变化等等。

格式为 `({ dispatch, history }, done) => unlistenFunction`。

注意：如果要使用 `app.unmodel()`，subscription 必须返回 unlisten 方法，用于取消数据订阅。



# dva.js 知识导图

- [Read "the dva.js Knowledgemap" in English](./README_en.md)
- ["the dva.js Knowledgemap" 日本語版](./README_ja.md)
> 注：如果你使用 dva@2，请先忽略这里的路由部分，待更新。

不知大家学 react 或 dva 时会不会有这样的疑惑：

- es6 特性那么多，我需要全部学会吗?
- react component 有 3 种写法，我需要全部学会吗?
- reducer 的增删改应该怎么写?
- 怎么做全局/局部的错误处理?
- 怎么发异步请求?
- 怎么处理复杂的异步业务逻辑?
- 怎么配置路由?
- ...

这篇文档梳理了基于 [dva-cli](https://github.com/dvajs/dva-cli) 使用 [dva](https://github.com/dvajs/dva) 的最小知识集，让你可以用最少的时间掌握创建类似 [dva-hackernews](https://github.com/dvajs/dva-hackernews) 的全部知识，并且不需要掌握额外的冗余知识。

# dva 知识地图

## 目录

* [JavaScript 语言](#javascript-语言)
  * [变量声明](#变量声明)
    * [const 和 let](#const-和-let)
    * [模板字符串](#模板字符串)
    * [默认参数](#默认参数)
  * [箭头函数](#箭头函数)
  * [模块的 Import 和 Export](#模块的-import-和-export)
  * [ES6 对象和数组](#es6-对象和数组)
    * [析构赋值](#析构赋值)
    * [对象字面量改进](#对象字面量改进)
    * [Spread Operator](#spread-operator)
  * [Promises](#promises)
  * [Generators](#generators)
* [React Component](#react-component)
  * [Stateless Functional Components](#stateless-functional-components)
  * [JSX](#jsx)
    * [Component 嵌套](#component-嵌套)
    * [className](#classname)
    * [JavaScript 表达式](#javascript-表达式)
    * [Mapping Arrays to JSX](#mapping-arrays-to-jsx)
    * [注释](#注释)
    * [Spread Attributes](#spread-attributes)
  * [Props](#props)
    * [propTypes](#proptypes)
    * [往下传数据](#往下传数据)
    * [往上传数据](#往上传数据)
  * [CSS Modules](#css-modules)
    * [理解 CSS Modules](#理解-css-modules)
    * [定义全局 CSS](#定义全局-css)
    * [classnames Package](#classnames-package)
* [Reducer](#reducer)
  * [增删改](#增删改)
  * [嵌套数据的增删改](#嵌套数据的增删改)
* [Effect](#effect)
  * [Effects](#effects)
    * [put](#put)
    * [call](#call)
    * [select](#select)
  * [错误处理](#错误处理)
    * [全局错误处理](#全局错误处理)
    * [本地错误处理](#本地错误处理)
  * [异步请求](#异步请求)
    * [GET 和 POST](#get-和-post)
    * [统一错误处理](#统一错误处理)
* [Subscription](#subscription)
  * [异步数据初始化](#异步数据初始化)
    * [path-to-regexp Package](#path-to-regexp-package)
* [Router](#router)
  * [Config with JSX Element (router.js)](#config-with-jsx-element-routerjs)
  * [Route Components](#route-components)
    * [通过 connect 绑定数据](#通过-connect-绑定数据)
    * [Injected Props (e.g. location)](#injected-props-eg-location)
  * [基于 action 进行页面跳转](#基于-action-进行页面跳转)
* [dva 配置](#dva-配置)
  * [Redux Middleware](#redux-middleware)
  * [history](#history)
    * [切换 history 为 browserHistory](#切换-history-为-browserhistory)
    * [去除 hashHistory 下的 _k 查询参数](#去除-hashhistory-下的-_k-查询参数)
* [工具](#工具)
  * [通过 dva-cli 创建项目](#通过-dva-cli-创建项目)

## JavaScript 语言

### 变量声明

#### const 和 let

不要用 `var`，而是用 `const` 和 `let`，分别表示常量和变量。不同于 `var` 的函数作用域，`const` 和 `let` 都是块级作用域。

```javascript
const DELAY = 1000;

let count = 0;
count = count + 1;
```

#### 模板字符串

模板字符串提供了另一种做字符串组合的方法。

```javascript
const user = 'world';
console.log(`hello ${user}`);  // hello world

// 多行
const content = `
  Hello ${firstName},
  Thanks for ordering ${qty} tickets to ${event}.
`;
```

#### 默认参数

```javascript
function logActivity(activity = 'skiing') {
  console.log(activity);
}

logActivity();  // skiing
```

### 箭头函数

函数的快捷写法，不需要通过 `function` 关键字创建函数，并且还可以省略 `return` 关键字。

同时，箭头函数还会继承当前上下文的 `this` 关键字。

比如：

```javascript
[1, 2, 3].map(x => x + 1);  // [2, 3, 4]
```

等同于：

```javascript
[1, 2, 3].map((function(x) {
  return x + 1;
}).bind(this));
```

### 模块的 Import 和 Export

`import` 用于引入模块，`export` 用于导出模块。

比如：

```javascript
// 引入全部
import dva from 'dva';

// 引入部分
import { connect } from 'dva';
import { Link, Route } from 'dva/router';

// 引入全部并作为 github 对象
import * as github from './services/github';

// 导出默认
export default App;
// 部分导出，需 import { App } from './file'; 引入
export class App extend Component {};
```

### ES6 对象和数组

#### 析构赋值

析构赋值让我们从 Object 或 Array 里取部分数据存为变量。

```javascript
// 对象
const user = { name: 'guanguan', age: 2 };
const { name, age } = user;
console.log(`${name} : ${age}`);  // guanguan : 2

// 数组
const arr = [1, 2];
const [foo, bar] = arr;
console.log(foo);  // 1
```

我们也可以析构传入的函数参数。

```javascript
const add = (state, { payload }) => {
  return state.concat(payload);
};
```

析构时还可以配 alias，让代码更具有语义。

```javascript
const add = (state, { payload: todo }) => {
  return state.concat(todo);
};
```

#### 对象字面量改进

这是析构的反向操作，用于重新组织一个 Object 。

```javascript
const name = 'duoduo';
const age = 8;

const user = { name, age };  // { name: 'duoduo', age: 8 }
```

定义对象方法时，还可以省去 `function` 关键字。

```javascript
app.model({
  reducers: {
    add() {}  // 等同于 add: function() {}
  },
  effects: {
    *addRemote() {}  // 等同于 addRemote: function*() {}
  },
});
```

#### Spread Operator

Spread Operator 即 3 个点 `...`，有几种不同的使用方法。

可用于组装数组。

```javascript
const todos = ['Learn dva'];
[...todos, 'Learn antd'];  // ['Learn dva', 'Learn antd']
```

也可用于获取数组的部分项。

```javascript
const arr = ['a', 'b', 'c'];
const [first, ...rest] = arr;
rest;  // ['b', 'c']

// With ignore
const [first, , ...rest] = arr;
rest;  // ['c']
```

还可收集函数参数为数组。

```javascript
function directions(first, ...rest) {
  console.log(rest);
}
directions('a', 'b', 'c');  // ['b', 'c'];
```

代替 apply。

```javascript
function foo(x, y, z) {}
const args = [1,2,3];

// 下面两句效果相同
foo.apply(null, args);
foo(...args);
```

对于 Object 而言，用于组合成新的 Object 。(ES2017 stage-2 proposal)

```javascript
const foo = {
  a: 1,
  b: 2,
};
const bar = {
  b: 3,
  c: 2,
};
const d = 4;

const ret = { ...foo, ...bar, d };  // { a:1, b:3, c:2, d:4 }
```

此外，在 JSX 中 Spread Operator 还可用于扩展 props，详见 [Spread Attributes](#spread-attributes)。

### Promises

Promise 用于更优雅地处理异步请求。比如发起异步请求：

```javascript
fetch('/api/todos')
  .then(res => res.json())
  .then(data => ({ data }))
  .catch(err => ({ err }));
```

定义 Promise 。

```javascript
const delay = (timeout) => {
  return new Promise(resolve => {
    setTimeout(resolve, timeout);
  });
};

delay(1000).then(_ => {
  console.log('executed');
});
```

### Generators

dva 的 effects 是通过 generator 组织的。Generator 返回的是迭代器，通过 `yield` 关键字实现暂停功能。

这是一个典型的 dva effect，通过 `yield` 把异步逻辑通过同步的方式组织起来。

```javascript
app.model({
  namespace: 'todos',
  effects: {
    *addRemote({ payload: todo }, { put, call }) {
      yield call(addTodo, todo);
      yield put({ type: 'add', payload: todo });
    },
  },
});
```

## React Component

###  Stateless Functional Components

React Component 有 3 种定义方式，分别是 `React.createClass`, `class` 和 `Stateless Functional Component`。推荐尽量使用最后一种，保持简洁和无状态。这是函数，不是 Object，没有 `this` 作用域，是 pure function。

比如定义 App Component 。

```javascript
function App(props) {
  function handleClick() {
    props.dispatch({ type: 'app/create' });
  }
  return <div onClick={handleClick}>${props.name}</div>
}
```

等同于：

```javascript
class App extends React.Component {
  handleClick() {
    this.props.dispatch({ type: 'app/create' });
  }
  render() {
    return <div onClick={this.handleClick.bind(this)}>${this.props.name}</div>
  }
}
```

### JSX

#### Component 嵌套

类似 HTML，JSX 里可以给组件添加子组件。

```html
<App>
  <Header />
  <MainContent />
  <Footer />
</App>
```

#### className

`class` 是保留词，所以添加样式时，需用 `className` 代替 `class` 。

```html
<h1 className="fancy">Hello dva</h1>
```

#### JavaScript 表达式

JavaScript 表达式需要用 `{}` 括起来，会执行并返回结果。

比如：

```javascript
<h1>{ this.props.title }</h1>
```

#### Mapping Arrays to JSX

可以把数组映射为 JSX 元素列表。

```javascript
<ul>
  { this.props.todos.map((todo, i) => <li key={i}>{todo}</li>) }
</ul>
```

#### 注释

尽量别用 `//` 做单行注释。

```javascript
<h1>
  {/* multiline comment */}
  {/*
    multi
    line
    comment
    */}
  {
    // single line
  }
  Hello
</h1>
```

#### Spread Attributes

这是 JSX 从 ECMAScript6 借鉴过来的很有用的特性，用于扩充组件 props 。

比如：

```javascript
const attrs = {
  href: 'http://example.org',
  target: '_blank',
};
<a {...attrs}>Hello</a>
```

等同于

```javascript
const attrs = {
  href: 'http://example.org',
  target: '_blank',
};
<a href={attrs.href} target={attrs.target}>Hello</a>
```

### Props

数据处理在 React 中是非常重要的概念之一，分别可以通过 props, state 和 context 来处理数据。而在 dva 应用里，你只需关心 props 。

#### propTypes

JavaScript 是弱类型语言，所以请尽量声明 propTypes 对 props 进行校验，以减少不必要的问题。

```javascript
function App(props) {
  return <div>{props.name}</div>;
}
App.propTypes = {
  name: React.PropTypes.string.isRequired,
};
```

内置的 prop type 有：

- PropTypes.array
- PropTypes.bool
- PropTypes.func
- PropTypes.number
- PropTypes.object
- PropTypes.string

#### 往下传数据

![](https://zos.alipayobjects.com/rmsportal/NAzeMyUoPMqxfRv.png)

#### 往上传数据

![](https://zos.alipayobjects.com/rmsportal/fiKKgDGuEJfSvxv.png)

### CSS Modules

<img src="https://zos.alipayobjects.com/rmsportal/mHVRpjNYhVuFdsS.png" width="150" style="background:#fff;" />

#### 理解 CSS Modules

一张图理解 CSS Modules 的工作原理：

![](https://zos.alipayobjects.com/rmsportal/SWBwWTbZKqxwEPq.png)

`button` class 在构建之后会被重命名为 `ProductList_button_1FU0u` 。`button` 是 local name，而 `ProductList_button_1FU0u` 是 global name 。**你可以用简短的描述性名字，而不需要关心命名冲突问题。**

然后你要做的全部事情就是在 css/less 文件里写 `.button {...}`，并在组件里通过 `styles.button` 来引用他。

#### 定义全局 CSS

CSS Modules 默认是局部作用域的，想要声明一个全局规则，可用 `:global` 语法。

比如：

```css
.title {
  color: red;
}
:global(.title) {
  color: green;
}
```

然后在引用的时候：

```javascript
<App className={styles.title} /> // red
<App className="title" />        // green
```

#### `classnames` Package

在一些复杂的场景中，一个元素可能对应多个 className，而每个 className 又基于一些条件来决定是否出现。这时，[classnames](https://github.com/JedWatson/classnames) 这个库就非常有用。

```javascript
import classnames from 'classnames';
const App = (props) => {
  const cls = classnames({
    btn: true,
    btnLarge: props.type === 'submit',
    btnSmall: props.type === 'edit',
  });
  return <div className={ cls } />;
}
```

这样，传入不同的 type 给 App 组件，就会返回不同的 className 组合：

```javascript
<App type="submit" /> // btn btnLarge
<App type="edit" />   // btn btnSmall
```

## Reducer

reducer 是一个函数，接受 state 和 action，返回老的或新的 state 。即：`(state, action) => state`

### 增删改

以 todos 为例。

```javascript
app.model({
  namespace: 'todos',
  state: [],
  reducers: {
    add(state, { payload: todo }) {
      return state.concat(todo);
    },
    remove(state, { payload: id }) {
      return state.filter(todo => todo.id !== id);
    },
    update(state, { payload: updatedTodo }) {
      return state.map(todo => {
        if (todo.id === updatedTodo.id) {
          return { ...todo, ...updatedTodo };
        } else {
          return todo;
        }
      });
    },
  },
};
```

### 嵌套数据的增删改

建议最多一层嵌套，以保持 state 的扁平化，深层嵌套会让 reducer 很难写和难以维护。

```javascript
app.model({
  namespace: 'app',
  state: {
    todos: [],
    loading: false,
  },
  reducers: {
    add(state, { payload: todo }) {
      const todos = state.todos.concat(todo);
      return { ...state, todos };
    },
  },
});
```

下面是深层嵌套的例子，应尽量避免。

```javascript
app.model({
  namespace: 'app',
  state: {
    a: {
      b: {
        todos: [],
        loading: false,
      },
    },
  },
  reducers: {
    add(state, { payload: todo }) {
      const todos = state.a.b.todos.concat(todo);
      const b = { ...state.a.b, todos };
      const a = { ...state.a, b };
      return { ...state, a };
    },
  },
});
```

## Effect

示例：

```javascript
app.model({
  namespace: 'todos',
  effects: {
    *addRemote({ payload: todo }, { put, call }) {
      yield call(addTodo, todo);
      yield put({ type: 'add', payload: todo });
    },
  },
});
```

### Effects

#### put

用于触发 action 。

```javascript
yield put({ type: 'todos/add', payload: 'Learn Dva' });
```

#### call

用于调用异步逻辑，支持 promise 。

```javascript
const result = yield call(fetch, '/todos');
```

#### select

用于从 state 里获取数据。

```javascript
const todos = yield select(state => state.todos);
```

### 错误处理

#### 全局错误处理

dva 里，effects 和 subscriptions 的抛错全部会走 `onError` hook，所以可以在 `onError` 里统一处理错误。

```javascript
const app = dva({
  onError(e, dispatch) {
    console.log(e.message);
  },
});
```

然后 effects 里的抛错和 reject 的 promise 就都会被捕获到了。

#### 本地错误处理

如果需要对某些 effects 的错误进行特殊处理，需要在 effect 内部加 `try catch` 。

```javascript
app.model({
  effects: {
    *addRemote() {
      try {
        // Your Code Here
      } catch(e) {
        console.log(e.message);
      }
    },
  },
});
```

### 异步请求

异步请求基于 whatwg-fetch，API 详见：https://github.com/github/fetch

#### GET 和 POST

```javascript
import request from '../util/request';

// GET
request('/api/todos');

// POST
request('/api/todos', {
  method: 'POST',
  body: JSON.stringify({ a: 1 }),
});
```

#### 统一错误处理

假如约定后台返回以下格式时，做统一的错误处理。

```javascript
{
  status: 'error',
  message: '',
}
```

编辑 `utils/request.js`，加入以下中间件：

```javascript
function parseErrorMessage({ data }) {
  const { status, message } = data;
  if (status === 'error') {
    throw new Error(message);
  }
  return { data };
}
```

然后，这类错误就会走到 `onError` hook 里。

## Subscription

`subscriptions` 是订阅，用于订阅一个数据源，然后根据需要 dispatch 相应的 action。数据源可以是当前的时间、服务器的 websocket 连接、keyboard 输入、geolocation 变化、history 路由变化等等。格式为 `({ dispatch, history }) => unsubscribe` 。

### 异步数据初始化

比如：当用户进入 `/users` 页面时，触发 action `users/fetch` 加载用户数据。

```javascript
app.model({
  subscriptions: {
    setup({ dispatch, history }) {
      history.listen(({ pathname }) => {
        if (pathname === '/users') {
          dispatch({
            type: 'users/fetch',
          });
        }
      });
    },
  },
});
```

#### `path-to-regexp` Package

如果 url 规则比较复杂，比如 `/users/:userId/search`，那么匹配和 userId 的获取都会比较麻烦。这是推荐用 [path-to-regexp](https://github.com/pillarjs/path-to-regexp) 简化这部分逻辑。

```javascript
import pathToRegexp from 'path-to-regexp';

// in subscription
const match = pathToRegexp('/users/:userId/search').exec(pathname);
if (match) {
  const userId = match[1];
  // dispatch action with userId
}
```

## Router

### Config with JSX Element (router.js)

```javascript
<Route path="/" component={App}>
  <Route path="accounts" component={Accounts}/>
  <Route path="statements" component={Statements}/>
</Route>
```

详见：[react-router](https://github.com/reactjs/react-router/blob/master/docs/guides/RouteConfiguration.md)

### Route Components

Route Components 是指 `./src/routes/` 目录下的文件，他们是 `./src/router.js` 里匹配的 Component。

#### 通过 connect 绑定数据

比如：

```javascript
import { connect } from 'dva';
function App() {}

function mapStateToProps(state, ownProps) {
  return {
    users: state.users,
  };
}
export default connect(mapStateToProps)(App);
```

然后在 App 里就有了 `dispatch` 和 `users` 两个属性。

#### Injected Props (e.g. location)

Route Component 会有额外的 props 用以获取路由信息。

- location
- params
- children

更多详见：[react-router](https://github.com/reactjs/react-router/blob/master/docs/API.md#injected-props)

### 基于 action 进行页面跳转

```javascript
import { routerRedux } from 'dva/router';

// Inside Effects
yield put(routerRedux.push('/logout'));

// Outside Effects
dispatch(routerRedux.push('/logout'));

// With query
routerRedux.push({
  pathname: '/logout',
  query: {
    page: 2,
  },
});
```

除 `push(location)` 外还有更多方法，详见 [react-router-redux](https://github.com/reactjs/react-router-redux#pushlocation-replacelocation-gonumber-goback-goforward)

## dva 配置

### Redux Middleware

比如要添加 redux-logger 中间件：

```javascript
import createLogger from 'redux-logger';
const app = dva({
  onAction: createLogger(),
});
```

注：onAction 支持数组，可同时传入多个中间件。

### history

#### 切换 history 为 browserHistory

```javascript
import { browserHistory } from 'dva/router';
const app = dva({
  history: browserHistory,
});
```

#### 去除 hashHistory 下的 _k 查询参数

```javascript
import { useRouterHistory } from 'dva/router';
import { createHashHistory } from 'history';
const app = dva({
  history: useRouterHistory(createHashHistory)({ queryKey: false }),
});
```

## 工具

### 通过 dva-cli 创建项目

先安装 dva-cli 。

```bash
$ npm install dva-cli -g
```

然后创建项目。

```bash
$ dva new myapp
```

最后，进入目录并启动。

```bash
$ cd myapp
$ npm start
```


## React + Redux 最佳实践

> 更新：我们基于此最佳实践做了一个封装方案：dva，可以简化使用 redux 和 redux-saga 时很多繁杂的操作。

![](https://camo.githubusercontent.com/21740ab2fdb2ba1504678bfddf39ab9943adfa39/68747470733a2f2f6f732e616c697061796f626a656374732e636f6d2f726d73706f7274616c2f506b4a564957464a62705a63776d532e706e67)

前端变化虽快，但其实一直都围绕这几个概念在转：

* URL - 访问什么页面
* Data - 显示什么信息
* View - 页面长成什么样
* Action - 对页面做了什么操作
* API Server - Data 数据的来源

在 redux 的生态圈内，每个环节有多种方案，比如 Data 可以是 `immutable` 或者 `plain object`，在你选了 `immutable` 之后，用 immutable.js 还是 seamless-immutable，以及是否用 redux-immutable 来辅助数据修改，都需要选择。

本文总结目前 react + redux 的最佳实践，解释原因，并提供可选方案。

心急的朋友可以直接看代码：https://github.com/sorrycc/github-stars

## 一、URL > Data

### 需求

routing

### 选择

`react-router` + `react-router-redux`: 前者是业界标准，后者可以同步 route 信息到 state，这样你可以在 view 根据 route 信息调整展现，以及通过 action 来修改 route 。

### 可选

无

## 二、Data

### 需求

为 redux 提供数据源，修改容易。

### 方案

`plain object`: 配合 combineReducer 已经可以满足需求。

同时在组织 Store 的时候，层次不要太深，尽量保持在 2 - 3 层。如果层次深，可以考虑用 updeep 来辅助修改数据。

### 可选

immutable.js: 通过自定义的 api 来操作数据，需要额外的学习成本。不熟悉 immutable.js 的可以先尝试用 seamless-immutable，JavaScript 原生接口，无学习门槛。

另外，不推荐用 redux-immutable 以及 redux-immutablejs，一是没啥必要，具体看他们的实现就知道了，都比较简单；更重要的是他们都改写了 combineReducer，会带来潜在的一些兼容问题。

## 三、Data > View

### 需求

数据的过滤和筛选。

### 方案

reselect: store 的 select 方案，用于提取数据的筛选逻辑，让 Component 保持简单。选 reselct 看重的是 可组合特性 和 缓存机制 。

### 可选

无

## 四、View 之 CSS 方案

### 需求

合理的 CSS 方案，考虑团队协作。

### 方案

css-modules: 配合 webpack 的 css-loader 进行打包，会为所有的 class name 和 animation name 加 local scope，避免潜在冲突。

直接看代码：

Header.jsx

``` javascript
import style from './Header.less';
export default () => <div className={style.normal} />;
```

Header.less

``` css
.normal { color: red; }
```

编译后，文件中的 `style.normal` 和 `.normal` 在会被重命名为类似 Header__normal___VI1de 。

### 可选

bem, rscss ，这两个都是基于约定的方案。但基于约定会带来额外的学习成本和不遍，比如 rscss 要求所有的 Component 都是两个词的连接，比如 Header 就必须换成类似 HeaderBox 这样。

radium，inline css 方案，没研究。

## 五、Action <> Store，业务逻辑处理

### 需求

统一处理业务逻辑，尤其是异步的处理。

### 方案

redux-saga: 用于管理 action，处理异步逻辑。可测试、可 mock、声明式的指令。

### 可选

redux-loop: 适用于相对简单点的场景，可以组合异步和同步的 action 。但他有个问题是改写了 `combineReducer`，会导致一些意想不到的兼容问题，比如我在特定场景下用不了 redux-devtool 。

redux-thunk, redux-promise 等: 相对原始的异步方案，适用于更简单的场景。在 action 需要组合、取消等操作时，会不好处理。

### saga 入门

在 saga 之前，你可能会在 action creator 里处理业务逻辑，虽然能跑通，但是难以测试。比如：

``` javascript
// action creator with thunking
function createRequest () {
  return (dispatch, getState) => {
    dispatch({ type: 'REQUEST_STUFF' });
    someApiCall(function(response) {
      // some processing
      dispatch({ type: 'RECEIVE_STUFF' });
    });
  };
}
```

然后组件里可能这样：

``` javascript
function onHandlePress () {
  this.props.dispatch({ type: 'SHOW_WAITING_MODAL' });
  this.props.dispatch(createRequest());
}
```

这样通过 redux state 和 reducer 把所有的事情串联到起来。

但问题是：
>Code is everywhere.

通过 saga，你只需要触发一个 action 。

``` javascript
function onHandlePress () {
  // createRequest 触发 action `BEGIN_REQUEST`
  this.props.dispatch(createRequest());
}
```

然后所有后续的操作都通过 saga 来管理。

``` javascript
function *hello() {
  // 等待 action `BEGIN_REQUEST`
  yield take('BEGIN_REQUEST');
  // dispatch action `SHOW_WAITING_MODAL`
  yield put({ type: 'SHOW_WAITING_MODAL' });
  // 发布异步请求
  const response = yield call(myApiFunctionThatWrapsFetch);
  // dispatch action `PRELOAD_IMAGES`, 附上 response 信息
  yield put({ type: 'PRELOAD_IMAGES', response.images });
  // dispatch action `HIDE_WAITING_MODAL`
  yield put({ type: 'HIDE_WAITING_MODAL' });
}
```

可以看出，调整之后的代码有几个优点：

* 所有业务代码都存于 saga 中，不再散落在各处
* 全同步执行，就算逻辑再复杂，看起来也不会乱

## 六、Data <> API Server

### 需求

异步请求。

### 方案

isomorphic-fetch: 便于在同构应用中使用，另外同时要写 node 和 web 的同学可以用一个库，学一套 api 。

然后通过 async + await 组织代码。

示例代码：

``` javascript
import fetch from 'isomorphic-fetch';
export async function fetchUser(uid) {
  return await fetch(`/users/${uid}`).then(res => res.json());
};
```

### 可选

reqwest

## 最终

![](https://camo.githubusercontent.com/068c4ff126977b861cff3338428bdde6927f7dad/68747470733a2f2f6f732e616c697061796f626a656374732e636f6d2f726d73706f7274616c2f43684d775a42755a6c614c725377652e706e67)

（完）
