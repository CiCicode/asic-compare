# 台灣 ASIC 設計服務 · 財務比較

三家具代表性的台灣 ASIC / IC 設計公司 — 世芯-KY、創意電子、聯發科 — 的季度財務數據一頁式儀表板，快速掌握營運趨勢。

## 網址

https://asic-compare.vercel.app

<img width="539" height="326" alt="image" src="https://github.com/user-attachments/assets/7ae6f099-05ce-4e28-9b42-e99fe22ce509" />
<img width="536" height="155" alt="image" src="https://github.com/user-attachments/assets/110c687f-6917-4b03-b135-0e3c8389550a" />

## 產業生態系總覽
```mermaid
flowchart TB
    subgraph EDA["EDA 供應商"]
        S[Synopsys]
        C[Cadence]
        M[Siemens EDA]
        A[Ansys]
    end

    subgraph IP["Silicon IP 供應商"]
        ARM[ARM]
        S_IP[Synopsys IP]
        C_IP[Cadence IP]
        O_IP[其他第三方 IP]
    end

    subgraph Fabless["Fabless 設計公司"]
        N[NVIDIA / AMD]
        Q[Qualcomm]
        M_MTK[MediaTek]
        BR[Broadcom]
        AM[Apple Silicon]
        HC[HPC / AI 晶片新創]
    end

    subgraph Foundry["晶圓代工廠"]
        TSMC[TSMC]
        S_Foundry[Samsung Foundry]
        GF[GlobalFoundries]
        UMC[UMC]
        SMIC[SMIC]
    end

    subgraph OSAT["封裝測試廠"]
        ASE[ASE]
        AMK[Amkor]
        JCET[JCET / STATS ChipPAC]
        PTI[PTI]
    end

    EDA --> Fabless
    IP --> Fabless
    Fabless --> Foundry
    Foundry --> OSAT
    Fabless --> OSAT

    subgraph Customer["終端客戶"]
        CSP[AWS / Azure / GCP<br/>雲端服務商]
        OEM[Apple / Dell / Tesla / ...<br/>品牌系統廠]
        SI[系統整合商<br/>System Integrator]
    end
```

## 為什麼這個專案有用？

- **一站式追蹤**：不用分別去公開資訊觀測站撈三家的季報，營收、毛利率、EPS 整理在同一頁
- **法說會紀要整合**：每季法說會重點直接寫在旁邊，不用再翻新聞稿
- **開源透明**：資料來源全標示公開資訊觀測站，數字可追溯、可驗證
- **自動化更新腳本**：內建批次更新按鈕，新季度資料可直接補充


## 資料來源

公開資訊觀測站 (mops.twse.com.tw)

