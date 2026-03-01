**悄悄滴在这里贴出代码**
<br />
<br />
<br />
**发现大家最近作业是不是有点多**
<br />
<br />
<br />
##### 只许借鉴啊！
<br />
<br />
#### 不要抄袭

### 不要抄袭

## 不要抄袭

## 代码用途与核心

这些 `.m` 文件是工程光学课程中的干涉/衍射仿真示例，核心思路是用 **光程差/相位差** 叠加得到强度分布：

1. `meshgrid` 生成屏面采样点。
2. 计算光源/孔到屏面的光程（或相位差）。
3. 用 `cos/sin` 或复振幅叠加得到强度 \(I = |E|^2\)。
4. 使用 `surf/plot` 进行二维或三维可视化。

### 文件说明（用途 + 核心）

- **EqualInclinationInterference.m**：等倾干涉（海丁格条纹）。核心是平行平板内折射角导致的光程差，得到同心圆条纹。
- **EqualInclinationInterferenceDynamic.m**：等倾干涉的动态演示，扫描平板厚度并用 `movie2avi` 导出动画。
- **EqualThicknessInterference.m**：等厚干涉（劈尖/牛顿条纹）。核心是厚度线性变化带来的光程差。
- **EqualThicknessInterferenceRoughFlatform.m**：等厚干涉叠加“凸/凹”局部形变，比较不同表面形貌的条纹差异。
- **FivePointInterference.m**：五点光源干涉。核心是 5 个点源复振幅叠加，得到四象限强度分布。
- **FraunhoferHole.m**：圆孔夫琅禾费衍射（Airy 斑）。核心公式使用 Bessel 函数。
- **FraunhoferSqueraHole.m**：方孔夫琅禾费衍射。核心是二维 sinc 函数的乘积。
- **FraunhoferTwoHoleDynamic.m**：双孔夫琅禾费衍射动态演示，改变孔间距并导出动画。
- **ThreePointInterference.m**：三点光源干涉。核心是三点源复振幅叠加，展示灰度干涉图样。
- **ThreePointInterferenceDynamic.m**：三点光源干涉的动态演示，扫描点源半径（可取消注释导出动画）。
- **ThreePointInterferenceOrigin.m**：固定半径的三点干涉静态版。
- **TwoPointInterference.m**：双点干涉在不同观察面位置下的差异，核心是两点源光程差。
- **YoungsDoubleSlitInterference.m**：杨氏双缝干涉，比较光源位置、缝距、波长变化对条纹的影响。
