# DCDC_DOWN_Converter_4_ISHI-KAI_OpenMPW_TR10-1
ISHI-KAI_Multiple_Projects_OpenMPW_TR10-1 向けの降圧型DCDCコンバータ（12v->5V）です。


# Members 
- [lufe](https://github.com/1uf3/vco)
    - VCO担当
- [noritsuna](https://github.com/noritsuna/DCDC_DOWN_Converter_4_ISHI-KAI_OpenMPW_TR10-1)
    - 降圧部担当


## 内容
- ![DCDC_DOWN_SLIDE_1](images/DCDC_down/slide1.png)
- ![DCDC_DOWN_SLIDE_2](images/DCDC_down/slide2.png)
- ![DCDC_DOWN_SLIDE_3](images/DCDC_down/slide3.png)

# 作成物

## vco
[lufe](https://github.com/1uf3/vco)担当

### xschem

#### inverter

![inverter](https://raw.githubusercontent.com/1uf3/vco/main/images/inverter.png)

#### buffer

![buffer](https://raw.githubusercontent.com/1uf3/vco/main/images/buffer.png)

#### vco

![vco](https://raw.githubusercontent.com/1uf3/vco/main/images/vco.png)

#### simulated vco hz

![simulated_vco_hz](https://raw.githubusercontent.com/1uf3/vco/main/images/simulated_vco_hz.png)

### klayout

![klayout_vco](https://raw.githubusercontent.com/1uf3/vco/main/images/klayout_vco.png)


## 降圧部
### xschem
- ![xschem_tb](images/xschem_tb.png)

#### simulation
- ![xschem_ngspice](images/xschem_ngspice.png)
- ![xschem_ngspice_cir](images/xschem_ngspice_cir.png)

### klayout
- ![klayout_dcdc_base](images/klayout_dcdc_base.png)


## 降圧型DCDCコンバータ
### xschem
- ![xschem_full](images/xschem_full.png)

#### simulation
- ![xschem_full_ngspice](images/xschem_full_ngspice.png)
- ![xschem_full_ngspice_cir](images/xschem_full_ngspice_cir.png)

### klayout
- ![klayout_dcdc_down](images/klayout_dcdc_down.png)


# WSL Image
上記の回路図やシミュレーション、レイアウト、DRC、LVSを実行するための環境をセットアップしたWSLイメージを用意しています。

- [WSL Image](https://www.noritsuna.jp/download/ubuntu2204_TR10-1.tar.xz)
    - ID: ishikai
    - Pass: ishikai

## Installing WSL Images
`wsl --import-in-place ubuntu2204_TR10-1 .\ubuntu2204_TR10-1\ext4.vhdx`

起動には"ubuntu2204_TR10-1.lnk"をご利用ください。  


## Deleting WSL Images
イメージも削除されるので注意してください。    

`wsl --unregister ubuntu2204_TR10-1`
