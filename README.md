将两个文件放在一起即可
module seven_segment_display(
    input wire reset,
    input wire clk,
    input wire [7:0] datain1,
    input wire [7:0] datain2,
    input wire [7:0] datain3,
    input wire [7:0] datain4,
    input wire [7:0] datain5,
    input wire [7:0] datain6,
    output wire enable,
    output wire databit,
    output wire shcp,
    output wire stcp
);

//num:
// 00001001;//9
// 00000001;//8
// 00011111;//7
// 01000001;//6
// 01001001;//5
// 10011001;//4
// 00001101;//3
// 00100101;//2
// 10011111;//1
// 00000011;//0
datin1-6分别对应开发板上的6个数字，代码中注释掉的二进制码对应的显示数字
