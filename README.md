# Verilog_digital_electronics.
The repository with my digital electronics and verilog exercises
<img width="730" height="802" alt="image" src="https://github.com/user-attachments/assets/d98df107-4755-452e-b61c-0bb95c3b9e2c" />
<img width="740" height="887" alt="image" src="https://github.com/user-attachments/assets/fd42a43c-0577-46db-ad26-18af17e47d5e" />
<img width="687" height="1023" alt="image" src="https://github.com/user-attachments/assets/06267d22-04d8-45eb-b664-7ecb35d3d5a8" />
<img width="682" height="933" alt="image" src="https://github.com/user-attachments/assets/d60d192d-c631-42fd-a42a-e34fb949580c" />
<img width="553" height="1022" alt="image" src="https://github.com/user-attachments/assets/e5532919-58c9-4fe1-8841-1855fabdfdd5" />
<img width="979" height="1057" alt="image" src="https://github.com/user-attachments/assets/484eaf91-f9ea-4405-9ba3-02a3818bf20c" />
<img width="1325" height="418" alt="image" src="https://github.com/user-attachments/assets/2057fd6d-8be2-416c-8958-ff4aec67bdc7" />
<img width="1259" height="475" alt="image" src="https://github.com/user-attachments/assets/acc0022c-9ae3-4981-af14-b40abcf68f78" />
<img width="524" height="625" alt="image" src="https://github.com/user-attachments/assets/89257fda-a331-4873-979b-a3d503ff7cec" />
<img width="1542" height="961" alt="image" src="https://github.com/user-attachments/assets/d8ee0829-8f47-42b7-aa8b-1486aa439204" />
<img width="580" height="355" alt="image" src="https://github.com/user-attachments/assets/21544158-09f1-4b69-be47-30bd03d0e014" />

<img width="1511" height="940" alt="image" src="https://github.com/user-attachments/assets/e09adecc-1526-4361-833b-b3271ff8eb0c" />
<img width="1538" height="442" alt="image" src="https://github.com/user-attachments/assets/937136ad-7085-4f59-aa41-2954a170393f" />
<img width="1088" height="704" alt="image" src="https://github.com/user-attachments/assets/ca980457-412c-46ac-8ca9-60ed6b815c7b" />
<img width="788" height="874" alt="image" src="https://github.com/user-attachments/assets/4ec7a2be-62ee-40fa-b39e-efc8a52b8229" />

<img width="1549" height="336" alt="image" src="https://github.com/user-attachments/assets/a519dbf1-453a-4b67-a2e6-dc97eb954326" />

module top_module (
    input  [1:0] A,
    input  [1:0] B,
    output       z
);

    assign z = (A == B);

endmodule
✔ Why this works
(A == B) is a Boolean expression.

If both 2-bit numbers are equal → expression becomes 1.

Otherwise → 0.

assign is perfect for combinational logic.

If you want the version using an always block, here it is too:

verilog
Copy code
module top_module (
    input  [1:0] A,
    input  [1:0] B,
    output reg   z
);

    always @(*) begin
        if (A == B)
            z = 1;
        else
            z = 0;
    end

endmodule

<img width="1024" height="683" alt="image" src="https://github.com/user-attachments/assets/728de64f-92b2-4581-94e1-811a6d3bf97c" />
<img width="1401" height="947" alt="image" src="https://github.com/user-attachments/assets/99fc8771-04b8-4dd9-b343-78747800555b" />

<img width="1508" height="872" alt="image" src="https://github.com/user-attachments/assets/811d7fd5-0f1e-4d76-b29f-4537afccadf6" />
<img width="646" height="692" alt="image" src="https://github.com/user-attachments/assets/aba2d1b2-aa7c-4e68-8bf1-47f3b1e54232" />

<img width="1518" height="1064" alt="image" src="https://github.com/user-attachments/assets/4e61c21e-11c1-4c48-9d68-0443fd9e7bc6" />
<img width="570" height="259" alt="image" src="https://github.com/user-attachments/assets/1d732419-7a8a-4776-b4a0-59872e25af2b" />
<img width="819" height="965" alt="image" src="https://github.com/user-attachments/assets/ee8e6795-ddf5-4e31-9196-0133a291279a" />




