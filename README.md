# -基因蛋白网络互作图的画图标准

Cytoscape  version 3.4.0  for windows (32bit)

##filling colour 蓝色 RGB(G) 137 208 245
##背景形状  圆形
##差异形状(diff)  菱形（需要选中diff那列，然后鼠标右键edit，再选中菱形）
    Mapping  Typt:  Discrete Mapping

##log2(FC) 选颜色
    红色代表上调基因，(红色：255.0.0)；
    绿色代表下调基因，(绿色：0.255.51)；
    还需要添加三条线：-1,0,1；
      -1：颜色绿色(0.255.51);
      0：颜色白色；
      1：颜色红色(255.0.0)
    Mapping Type: Continuous Mapping
  
##设置size(根据FDR，首先要勾选lock node width and height才能设置)
  Default Value:  20.0;
  Mapping Type: Continuous Mapping
  Current Mapping:
    set min and max:  min:1.0E-8;max:1;
  当最左边Handle Positions and Value为0时：Node Size为80；
  当最右边Handle Positions and Value为1时：Node Size为30；
  再 add 一条线，此线为FDR分界点(Handle Size 默认为0.05)，此时Node Size设置为50
