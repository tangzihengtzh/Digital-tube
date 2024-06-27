将两个文件放在一起即可<br>
module seven_segment_display(<br>
    input wire reset,<br>
    input wire clk,<br>
    input wire [7:0] datain1,<br>
    input wire [7:0] datain2,<br>
    input wire [7:0] datain3,<br>
    input wire [7:0] datain4,<br>
    input wire [7:0] datain5,<br>
    input wire [7:0] datain6,<br>
    output wire enable,<br>
    output wire databit,<br>
    output wire shcp,<br>
    output wire stcp<br>
);<br>

//num:<br>
// 00001001;//9<br>
// 00000001;//8<br>
// 00011111;//7<br>
// 01000001;//6<br>
// 01001001;//5<br>
// 10011001;//4<br>
// 00001101;//3<br>
// 00100101;//2<br>
// 10011111;//1<br>
// 00000011;//0<br>
datin1-6分别对应开发板上的6个数字，代码中注释掉的二进制码对应的显示数字<br>
