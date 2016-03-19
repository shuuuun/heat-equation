# heat-equation
断熱材で囲まれた物体の端を熱し、その熱が物体を通過する伝熱速度は、熱の流れに垂直な断面積に比例することを表した方程式である。
熱伝導方程式から弱形式を算出し、FreeFem++というフリーソフトを用いて計算し、図式化した。  
・熱伝導方程式   
(d:partial differentiation  　
\int:integralとする)  
  
du/dt(x,t)-Δu(x,t)=f(x,t)   in Ω*(0,T]  
u(x,t)=g(x,t) on (0,T]  
du/dn(x,t)=0  
u(x,0)=u0(x) in Ω  
弱形式の算出:  
du/dt(x,t)-Δu(x,t)=f(x,t)⇔{u^(n+1)-u^n}/p=Δu^(n+1)+f  
両辺にテスト関数vをかけて積分すると、  
\int u^(n+1) *vdx+p\int ∇u^(n+1) *∇vdx-\int u^n *vdx =0  
  
環境  
mac OS X 10.9.5  
FreeFem++ ver.3.37  
mi ver.2.1.12r3  
動作方法  
FreeFem++をインストール後、choose a edp script と表示されるので特定のファイルをダブルクリックで動作します。
