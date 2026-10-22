程序化积雨云生成器 (Procedural Cumulonimbus Generator)
这是一个完全基于纯前端（原生 JavaScript + SVG）编写的程序化积雨云天空盒生成管线。无需任何第三方框架或依赖，直接在浏览器中打开即可运行。

项目从一个简单的圆点线稿开始，经过多次迭代，最终演变成了一个具备完整光影、景深透视、并且可以导出透明资产的天空盒生成器。

核心特性
纯数学驱动：云朵形态完全由伪随机函数与数学公式生成，无外部图片资源。

全参数实时调节：右侧面板提供数十个滑块，可实时调整云层高度、宽度、收束感、渐变强度、光照亮度等。

真实的光影材质：基于 55 度斜射光源计算，云顶带有极淡的暖白色高光边，云底呈现深邃的背光阴影。

极致的随机分布：云团的水平间距、叠放遮挡顺序、高度差均引入了离散化随机权重，打破了死板的排列感。

空间景深 (空气透视)：远处的云更小、透明度更高，近处的云更大、更清晰。

自由拖拽：按住鼠标（或触摸屏）即可左右滑动，欣赏全景天空。

导出透明云：一键剥离天空背景，将当前云层渲染为高清的透明 PNG 图像，方便作为素材合成到其他图片或游戏引擎中。

🚀 如何使用
双击在任何现代浏览器（Chrome, Edge, Safari, Firefox）中打开。

在右侧折叠面板中调节各项参数，或点击 “🎲 重新生成天空” 获取全新的云朵分布。

点击 “📥 导出透明云 (PNG)” 保存无背景的云层素材。

🛠️ 技术栈
HTML5 / CSS3 (原生 UI 与 折叠面板)

SVG (Scalable Vector Graphics) (核心渲染引擎，利用 Radial Gradient 实现体积光影)

Vanilla JavaScript (生成算法、交互逻辑)

Canvas API (用于导出 PNG 时进行光栅化)

📜 开源协议 (MIT License)
本项目采用 MIT 协议开源，你可以自由地使用、修改、分发，甚至用于商业项目。

text
MIT License

Copyright (c) 2024 Procedural Cumulonimbus Skybox

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


“In memory of Bob Ross. Happy little clouds. We don't make mistakes, just happy little accidents.”