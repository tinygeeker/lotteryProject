# 🎉 抽奖系统集合

## 📁 项目结构

```
lottoProject/
├── index.html                 # 首页
├── README.md                  # 项目说明
├── LICENSE                    # MIT License
├── config/
│   └── lottery_config.json    # 抽奖配置文件
├── lottery-grid/              # 九宫格抽奖
│   ├── native/                # 原生实现
│   └── vue/                   # Vue实现
├── lottery-wheel/             # 转盘抽奖
│   └── native/                # 原生实现
├── lottery-scratch/           # 刮刮乐抽奖
│   └── native/                # 原生实现
├── lottery-egg/               # 砸金蛋抽奖
│   ├── native/                # 原生实现
│   └── vue/                   # Vue实现
└── lottery-screen/            # 年会大屏抽奖
    ├── native/                # 原生实现
    └── vue/                   # Vue实现
```

## ✨ 功能特点

- 🎯 **多种抽奖类型**：九宫格、转盘、刮刮乐、砸金蛋、年会大屏抽奖
- 🎨 **现代化UI**：科技感设计，响应式布局
- ⚙️ **JSON配置**：通过config/lottery_config.json统一配置奖品
- 🔧 **双实现方式**：原生JavaScript和Vue.js实现
- 📱 **响应式设计**：适配不同屏幕尺寸
- 🎭 **动画效果**：流畅的抽奖动画和过渡效果
- 🏆 **中奖记录**：右侧实时显示中奖结果和历史记录
- 🎊 **年会大屏**：支持一次抽取多人
- 🔨 **砸金蛋特效**：真实的锤子敲击效果
- 🎉 **刮刮乐**：模拟真实刮奖体验

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
```

### 3. 访问项目

打开浏览器，访问：`http://localhost:8000`

## ⚙️ 配置说明

### 奖品配置

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

## 🎮 使用指南

1. **选择抽奖类型**：在首页点击对应抽奖类型的卡片
2. **开始抽奖**：点击抽奖按钮
3. **查看结果**：中奖结果会显示在右侧
4. **查看历史**：右侧面板会记录所有中奖历史
5. **年会大屏**：可设置一次抽取多人

## 🛠 技术实现

- **前端**：HTML5, CSS3, JavaScript, Vue.js
- **样式**：Flexbox布局，CSS动画
- **数据**：JSON配置文件
- **响应式**：媒体查询适配不同设备

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 🤝 贡献

欢迎提交 Issue 和 Pull Request 来改进这个项目！

## 🌟 鸣谢

- 感谢所有贡献者的努力
- 感谢 Vue.js 提供的优秀框架

---

🎉 祝大家好运，抽到心仪的奖品！

Powered by [tinygeeker](https://github.com/tinygeeker) 🚀