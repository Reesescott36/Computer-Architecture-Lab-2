# Computer-Architecture-Lab-2
module Lab2 (I,O);
input [7:0]I;
output [0:0]O;
reg [0:0]O;

integer i;
always @(I or O) begin
O[0]=0;
	for(i=0;i<5;i=i+1)
		if(I[i]==1&&I[i+1]==0&&I[i+2]==0&&I[i+3]==1)
		O[0]=1;
end
endmodule
