# 🎉 智能抽奖系统集合

## 📁 项目结构

```
lotteryProject/
├── index.html                 # 首页
├── README.md                  # 项目说明
├── LICENSE                    # MIT License
├── config/
│   ├── index.html             # 配置管理页面
│   └── lottery_config.json    # 抽奖配置文件
├── lottery-grid/              # 九宫格抽奖
│   ├── native/                # 原生实现
│   └── vue/                   # Vue实现
├── lottery-screen/            # 年会大屏抽奖
│   ├── native/                # 原生实现
│   └── vue/                   # Vue实现
├── lottery-wheel/             # 转盘抽奖
│   ├── native/                # 原生实现
│   └── vue/                   # Vue实现
├── lottery-scratch/           # 刮刮乐抽奖
│   ├── native/                # 原生实现
│   └── vue/                   # Vue实现
├── lottery-egg/               # 砸金蛋抽奖
│   ├── native/                # 原生实现
│   └── vue/                   # Vue实现
├── lottery-box/               # 抽奖箱
│   ├── native/                # 原生实现
│   └── vue/                   # Vue实现
├── lottery-gashapon/          # 扭蛋机
│   └── native/                # 原生实现
├── lottery-flip/              # 翻牌抽奖
│   ├── native/                # 原生实现
│   └── vue/                   # Vue实现
├── lottery-slot/              # 老虎机
│   └── native/                # 原生实现
├── lottery-redpack/           # 红包雨
│   └── native/                # 原生实现
├── lottery-password/          # 口令抽奖
│   └── native/                # 原生实现
└── lottery-welfare/           # 福彩抽奖
    └── native/                # 原生实现
```

## ✨ 功能特点

- 🎯 **多种抽奖类型**：九宫格、年会大屏、转盘、刮刮乐、砸金蛋、抽奖箱、扭蛋机、翻牌抽奖、老虎机、红包雨、口令抽奖、福彩抽奖
- 🎨 **现代化UI**：科技感设计，渐变色彩，流畅动画
- ⚙️ **统一配置管理**：通过配置页面管理所有抽奖的奖品和设置
- 🔧 **双实现方式**：原生JavaScript和Vue.js实现（部分模块）
- 📱 **响应式设计**：适配不同屏幕尺寸，支持移动设备
- 🎭 **丰富动画效果**：流畅的抽奖动画、过渡效果、粒子特效
- 🏆 **中奖记录**：实时显示中奖结果和历史记录
- 🎊 **年会大屏**：支持一次抽取多人，适合大型活动
- 🔨 **砸金蛋特效**：真实的锤子敲击效果和破碎动画
- 🎉 **刮刮乐**：模拟真实刮奖体验，支持福利彩票玩法
- 🎁 **红包雨**：互动性强的红包雨效果，支持点击抢红包
- 🎰 **老虎机**：经典老虎机玩法，拉动拉杆获取中奖组合
- 🎮 **扭蛋机**：模拟真实扭蛋机，透明容器和球动画效果
- 🃏 **翻牌抽奖**：3D翻牌效果，点击卡片查看是否中奖
- 🔑 **口令抽奖**：输入正确口令参与抽奖，支持自定义口令
- 🎫 **福彩抽奖**：模拟福利彩票玩法，匹配号码赢取奖品

## 🚀 快速开始

### 1. 克隆项目

```bash
git clone <repository-url>
cd lotteryProject
```

### 2. 启动本地服务器

```bash
# 使用Python 3
python -m http.server 8000

# 或使用Python 2
python -m SimpleHTTPServer 8000

# 或使用Node.js
npx http-server -p 8000

# 或使用PHP
php -S localhost:8000
```

### 3. 访问项目

打开浏览器，访问：`http://localhost:8000`

## ⚙️ 配置说明

### 1. 统一配置管理

访问 `http://localhost:8000/config/index.html` 进入配置管理页面，可统一管理所有抽奖的奖品配置。

### 2. 手动配置

编辑 `config/lottery_config.json` 文件，配置奖品信息：

```json
{
  "prizes": [
    {
      "id": 1,
      "name": "一等奖",
      "count": 1,
      "probability": 0.01,
      "image": ""
    },
    {
      "id": 2,
      "name": "二等奖",
      "count": 2,
      "probability": 0.05,
      "image": ""
    }
    // 更多奖品...
  ]
}
```

### 配置项说明

- `id`：奖品ID
- `name`：奖品名称
- `count`：奖品数量
- `probability`：中奖概率（0-1之间）
- `image`：奖品图片路径（可选）

## 项目预览

![donate](https://tinygeeker.github.io/assets/preview/0000000008.png)

## 🎮 使用指南

### 1. 选择抽奖类型

在首页点击对应抽奖类型的卡片，进入抽奖页面。

### 2. 开始抽奖

- **九宫格抽奖**：点击开始按钮，指针随机停在奖品格内
- **年会大屏抽奖**：点击开始按钮，滚动显示参与人员，点击停止抽取中奖者
- **转盘抽奖**：点击开始按钮，指针旋转后停在对应奖品区域
- **刮刮乐抽奖**：用鼠标刮开涂层查看中奖结果
- **砸金蛋抽奖**：点击金蛋砸开，查看是否中奖
- **抽奖箱**：点击抽取按钮，随机抽取奖品
- **扭蛋机**：点击转动按钮，获取随机奖品
- **翻牌抽奖**：点击卡片翻牌，查看是否中奖
- **老虎机**：点击拉杆按钮，获取中奖组合
- **红包雨**：点击飘落的红包，查看中奖结果
- **口令抽奖**：输入正确口令参与抽奖
- **福彩抽奖**：生成号码，检查是否与中奖号码匹配

### 3. 查看结果

- 中奖结果会实时显示在页面上
- 中奖记录会保存在页面的中奖记录区域
- 部分抽奖类型会有动画效果和弹窗提示

## 🛠 技术实现

- **前端**：HTML5, CSS3, JavaScript, Vue.js
- **样式**：CSS Grid布局，Flexbox布局，CSS动画和过渡效果
- **数据**：JSON配置文件，本地存储
- **响应式**：媒体查询适配不同设备
- **动画**：CSS关键帧动画，JavaScript动画，Canvas绘制
- **交互**：事件监听，DOM操作，用户交互反馈
- **随机**：随机数生成，概率计算

## 📱 响应式设计

- **桌面端**：4列网格布局，完整功能和动画效果
- **平板端**：2-3列网格布局，适配中等屏幕尺寸
- **移动端**：单列布局，优化触摸交互，简化动画效果

## 项目贡献

如果你觉得项目有用，就请我喝杯奶茶吧。 :tropical_drink:

![donate](https://tinygeeker.github.io/assets/user/donate.jpg)

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 🤝 贡献

欢迎提交 Issue 和 Pull Request 来改进这个项目！

### 贡献指南

1. Fork 本仓库
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开一个 Pull Request

## 🌟 鸣谢

- 感谢所有贡献者的努力
- 感谢 Vue.js 提供的优秀框架
- 感谢现代前端技术的发展，使得这些交互效果成为可能

## 📞 联系方式

- 项目作者：tinygeeker
- GitHub：[https://github.com/tinygeeker](https://github.com/tinygeeker)

---

🎉 祝大家好运，抽到心仪的奖品！

Powered by [tinygeeker](https://github.com/tinygeeker) 🚀