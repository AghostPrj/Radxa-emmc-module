<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Radxa-emmc-module](#radxa-emmc-module)
  - [版本(version)](#%E7%89%88%E6%9C%ACversion)
  - [原理图(schematic)](#%E5%8E%9F%E7%90%86%E5%9B%BEschematic)
  - [物料表(BOM)](#%E7%89%A9%E6%96%99%E8%A1%A8bom)
  - [生产文件(factory files)](#%E7%94%9F%E4%BA%A7%E6%96%87%E4%BB%B6factory-files)
    - [生产工艺需求(factory capacity)](#%E7%94%9F%E4%BA%A7%E5%B7%A5%E8%89%BA%E9%9C%80%E6%B1%82factory-capacity)
    - [生产文件使用说明](#%E7%94%9F%E4%BA%A7%E6%96%87%E4%BB%B6%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E)
    - [factory files usage](#factory-files-usage)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# Radxa-emmc-module

RADXA 3/4/5 emmc模块PCB    
emmc module pcb design for radxa 3/4/5

## 版本(version)

| 版本(version) | 更新日期(Date) |                                                                              更新说明(update desc.)                                                                              |
|:-----------:|:----------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|     v1      | 2021.11.17 |                                                                           第一版<p>the first version                                                                            |
|    v1.1     | 2022.05.09 |                                                                         修复过孔未盖油<p>fix via not tented                                                                         |
|    V2.0     | 2022.09.24 |               重新设计，修复焊盘过小导致的焊接难度增加，取消不必要的电容焊盘，将电容封装改为0402<p> redesign pcb, reduce soldering difficulty, remove optional capacity, use 0402 cap instead of 0603               |
|    V2.1     | 2022.10.26 | 重新设计pcb，将贴片电阻封装改为0402，并且将所有非emmc芯片的器件移动到底面，缩短了板子长度<p> redesign pcb, use 0402 resistance instead of 0603, move all component except emmc chip to bottom side, and reduce size |

## 原理图(schematic)

| 版本(version) |                   原理图(schematic)                   |
|:-----------:|:--------------------------------------------------:|
|    V1.1     |   [emmc-module-v1.1-sch](./images/sch-v1.1.png)    |
|    V2.0     | [emmc-module-v2.0-sch](./sch/emmc-module-V2.0.pdf) |
|    V2.1     |                    same as V2.0                    |

## 物料表(BOM)

| 版本(version) |                       物料表(BOM)                        |
|:-----------:|:-----------------------------------------------------:|
|    V1.1     | [emmc-module-v1.1-bom](./bom/emmc-module-V1.1-bom.md) |
|    V2.0     | [emmc-module-v2.0-bom](./bom/emmc-module-V2.0-bom.md) |
|    V2.1     | [emmc-module-v2.1-bom](./bom/emmc-module-V2.1-bom.md) |

## 生产文件(factory files)

gerber以及钻孔文件(gerber and drill files)

| 版本(version) |                 生产文件(factory files)                  |
|:-----------:|:----------------------------------------------------:|
|    V1.1     | [emmc-module-v1.1](./factory-files/emmc_module-V1.1) |
|    V2.0     | [emmc-module-v2.0](./factory-files/emmc-module-v2.0) |
|    V2.0     | [emmc-module-v2.1](./factory-files/emmc-module-v2.1) |

### 生产工艺需求(factory capacity)

4层pcb， 线宽、间距6mil，过孔内径0.2mm外径0.45mm  
4 layer pcb, 6mil line width and distance, via hole 0.2mm, via diameter 0.45mm

### 生产文件使用说明

1. 克隆或下载本仓库
2. 选择你需要的版本，将文件夹压缩为一个zip压缩包
3. 将压缩包交给PCB厂家生产

### factory files usage

1. clone or download this repo
2. choose which version you want to use and then compress it as a zip file
3. send the zip file to pcb factory