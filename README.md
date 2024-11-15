# antd-access

## 进度

- [x] 1. 创建前后端项目. 视频地址: [https://www.bilibili.com/video/BV1Bp4y1s7xQ/](https://www.bilibili.com/video/BV1Bp4y1s7xQ/)
- [x] 2. 前端项目的结构.以及创建页面. 视频地址: [https://www.bilibili.com/video/BV1Xv4y1Z72e/](https://www.bilibili.com/video/BV1Xv4y1Z72e/)
- [x] 3. 创建列表页面, 然后编写测试用例. 视频地址: [https://www.bilibili.com/video/BV19K4y1W7Gs/](https://www.bilibili.com/video/BV19K4y1W7Gs/)
- [x] 4. 开发思路及规划. 视频地址: [https://www.bilibili.com/video/BV1wz4y1D7dK/](https://www.bilibili.com/video/BV1wz4y1D7dK/)
- [x] 5. 角色界面的新建,编辑,删除. 视频地址: [https://www.bilibili.com/video/BV1Yv4y1o78w/](https://www.bilibili.com/video/BV1Yv4y1o78w/)
- [x] 6. 角色界面的 E2E 测试,优化,以及增加国际化的代码. 视频地址: [https://www.bilibili.com/video/BV1ZV411q7k3/](https://www.bilibili.com/video/BV1ZV411q7k3/)
- [x] 7. 菜单界面的 CRUD. 视频地址: [https://www.bilibili.com/video/BV1F5411K7Jb/](https://www.bilibili.com/video/BV1F5411K7Jb/)
- [x] 8. 菜单界面的 E2E 测试,优化. 视频地址: [https://www.bilibili.com/video/BV1GZ4y1P7tF/](https://www.bilibili.com/video/BV1GZ4y1P7tF/)
- [x] 9. 整体菜单与菜单数据的联动,补充之前菜单的国际化的缺失部分. 视频地址: [https://www.bilibili.com/video/BV1Sv411h7FS/](https://www.bilibili.com/video/BV1Sv411h7FS/)
- [x] 10. 用户界面的 CRUD. 视频地址: [https://www.bilibili.com/video/bv1oi4y1N7X2](https://www.bilibili.com/video/bv1oi4y1N7X2)
- [x] 11. 用户界面的 E2E 测试,优化. 视频地址: [https://www.bilibili.com/video/bv1Ry4y177db](https://www.bilibili.com/video/bv1Ry4y177db)
- [x] 12. 给角色分配菜单. 视频地址: [https://www.bilibili.com/video/BV1bZ4y1w7Sb/](https://www.bilibili.com/video/BV1bZ4y1w7Sb/)
- [x] 13. 给用户分配角色. 视频地址: [https://www.bilibili.com/video/BV11h411Q7Bj/](https://www.bilibili.com/video/BV11h411Q7Bj/)
- [x] 14. 分配菜单的 E2E 测试. 视频地址: [https://www.bilibili.com/video/BV1Qi4y1P7pZ/](https://www.bilibili.com/video/BV1Qi4y1P7pZ/)

## 小阶段总结

### 1-14 期 总结:

搭建了简单的框架,大致实现了角色+菜单+用户的一个联动, 使用 Mock 来模拟接口返回数据, Cypress 模拟 E2E 测试. 需要改进的地方: 1. 视频的时长需要控制一下.现在的时长基本都超过了 40 分钟. 2. 关于界面的美化, 需要稍微注意一点.

## 项目结构

```
.
├── package.json                 -- 这个就是项目配置相关 依赖包,名称,url ,命令脚本
├── tsconfig.json                -- 这个主要就是typescript 编译配置相关的东西
├── config                       -- 对项目在运行过程的一些配置.(静态配置)
    ├── config.ts                -- 项目主配置文件入口
    ├── routes.ts                -- 路由配置文件.
    ├── proxy.ts                 -- 代理文件
    └── defaultSettigns.ts       -- 默认配置
├── mock                         -- 前端模拟后端接口返回.
├── public                       -- logo . 一些图片.
├── src                          -- 我们的源码,我们主要在这里编码
    ├── components               -- 项目组件的存放地方. 推荐存放全局组件.
    ├── e2e                      -- 端到端的测试文件.
    ├── locales                  -- 国际化文件存放地方.
    ├── models                   -- 存放model. dva model 以及 umi-plugin-model  .
    ├── pages                    -- 页面的存放地方.
    ├── services                 -- 服务的存放地方.对于前端来说,请求API.以及一些其他的操作.
    ├── utils                    -- 工具文件
    ├── app.tsx                  -- 项目配置(动态配置)
    ├── access.ts                -- 权限定义文件
    └── typing.d.ts              -- 全局的一些类型.
```

1.目录结构

2.umi 增加页面  routes.ts路由里添加页面  menu 里 添加菜单

3.创建页面 pages 下面 创建文件夹  index.tsx   里面 添加组件 以及 组件属性   request 读数据 mock 里定义api函数 就要 services 里创建一个链接函数  注意异步

5.servoces Api 里定义 type  添加组件  看源码 复制




### B 站 BV 号

```
14. 分配菜单的 E2E 测试. BV1Qi4y1P7pZ
13. 分配菜单E2E. BV11h411Q7Bj
12. 给角色分配菜单. BV1bZ4y1w7Sb
11. 用户 E2E. bv1Ry4y177db
10. 用户界面 CRUD. bv1oi4y1N7X2
9. 菜单联动. BV1Sv411h7FS
8. 菜单 E2E. BV1GZ4y1P7tF
7. 菜单 CRUD. BV1F5411K7Jb
6. 角色界面 E2E. BV1ZV411q7k3
5. 角色界面 CRUD . BV1Yv4y1o78w
4. 开发思路及规划. BV1wz4y1D7dK
3. 角色界面 CRUD . BV19K4y1W7Gs
```
