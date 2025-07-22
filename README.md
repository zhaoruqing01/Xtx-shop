# Xtx-shop 电商平台
Xtx-shop 是一个基于 Vue 3 构建的现代化电商平台，采用了最新的前端技术栈，提供了完整的商品展示、购物车、结算、订单管理等电商核心功能。项目注重用户体验与代码可维护性，适合作为电商类应用的前端解决方案。
## 项目特点
- 技术前沿：基于 Vue 3 + Vite 构建，结合 Pinia 状态管理和 Vue Router 路由管理，采用 Composition API 语法风格
- 组件化设计：封装了通用组件（如商品规格选择器、图片预览组件），实现代码复用与维护性提升
- 响应式布局：适配不同屏幕尺寸，提供一致的用户体验
- 性能优化：实现图片懒加载、路由懒加载等性能优化策略
- 完整功能：包含商品展示、分类浏览、详情查看、购物车、结算支付、会员中心等核心电商功能
- 规范开发：使用 ESLint 进行代码校验，保持代码风格一致
## 技术栈
### 技术 / 工具	版本	说明
- Vue	^3.2.45	前端框架
- Vite	^4.0.0	构建工具
- Vue Router	^4.1.6	路由管理
- Pinia	^2.0.28	状态管理
- Element Plus	^2.2.28	UI 组件库
- Axios	^1.2.6	网络请求
- Sass	^1.57.1	CSS 预处理器
- @vueuse/core	^9.12.0	Vue 工具函数库
## 快速开始
### 环境要求
Node.js >= 14.0.0
npm >= 6.0.0 或 yarn >= 1.22.0
### 安装步骤
克隆仓库
git clone https://github.com/zhaoruqing01/Xtx-shop.git
cd Xtx-shop

### 安装依赖
- npm install
 或使用yarn
- yarn install

### 启动开发服务器
- npm run dev
或使用yarn
- yarn dev

## 访问应用
打开浏览器访问 http://localhost:5173（默认端口，具体以终端输出为准）
### 生产构建
- npm run build
 或使用yarn
- yarn build

### 构建产物会生成在 dist 目录下，可部署至服务器。
## 项目结构
```
plaintext
Xtx-shop/
├── public/               # 静态资源
├── src/
│   ├── apis/             # 接口请求函数
│   │   ├── detail.js     # 商品详情相关接口
│   │   └── home.js       # 首页相关接口
│   ├── components/       # 通用组件
│   │   ├── ImageView/    # 图片预览组件
│   │   └── XtxSku/       # 商品规格选择组件
│   ├── directives/       # 自定义指令
│   │   └── index.js      # 懒加载指令
│   ├── router/           # 路由配置
│   │   └── index.js      # 路由规则定义
│   ├── stores/           # Pinia状态管理
│   ├── styles/           # 样式文件
│   │   └── common.scss   # 全局样式
│   ├── utils/            # 工具函数
│   │   └── http.js       # Axios封装
│   ├── views/            # 页面组件
│   │   ├── Detail/       # 商品详情页
│   │   ├── Home/         # 首页
│   │   ├── CartList/     # 购物车页面
│   │   └── ...           # 其他页面
│   ├── App.vue           # 根组件
│   └── main.js           # 入口文件
├── .eslintrc.js          # ESLint配置
├── index.html            # 入口HTML
├── package.json          # 项目依赖配置
└── vite.config.js        # Vite配置
```
## 核心功能模块
### 首页模块
- 轮播图展示
- 新鲜好物推荐
- 人气商品展示
### 商品分类导航
- 商品模块
- 商品列表与筛选
- 商品详情展示
- 商品规格选择
- 商品图片预览
### 购物车模块
- 加入购物车
- 购物车商品管理（增删改查）
- 购物车商品结算
### 订单模块
- 订单创建
- 支付流程
- 订单查询与管理
### 会员中心
- 个人信息展示
- 我的订单查询
### 自定义指令
- v-img-lazy：图片懒加载指令，基于 @vueuse/core 的 useIntersectionObserver 实现，当图片进入视口时加载图片资源。
### 组件说明
- XtxImageView：图片预览组件，支持多图切换预览
- XtxSku：商品规格选择组件，处理商品多规格选择逻辑，包括规格联动与库存判断
## 许可证
本项目基于 Apache License 2.0 许可证开源，详情参见 LICENSE 文件。
## 开发规范
- 代码风格遵循 ESLint 配置，提交代码前请运行 npm run lint 进行校验
- 组件命名采用 PascalCase 风格（如 XtxSku）
- 工具函数与接口函数采用 camelCase 风格
- 提交信息请遵循 Angular 提交规范，便于版本管理与日志生成
## 致谢
- Vue.js - 优秀的前端框架
- Element Plus - 提供丰富的 UI 组件
- Vite - 快速的构建工具
- Pinia - 简洁的状态管理方案
