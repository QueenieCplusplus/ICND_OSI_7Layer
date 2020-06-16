# ICND OSI 7 Layer

# OSI 七 層

上三層 （應用）              

                               App

                          Presentation
                          
                             Session


下四層 （資料流）                

                            Transport
                               
                             Network
                               
                             DataLink
                             
                             Physical


資料網路的目的在於連接內部的所有電腦和電腦網路系統，讓員工不分時間、地點、主機，隨時能取得關資訊，提高生產力。也基於此，大家不必為了取得工作所需資料而齊聚一堂。

使用者群組的策略經營：

* 總公司

指的是該處每一位使用者共同組成一個區域網路 LAN，而公司中大多資料也儲存於此，它可能是一棟包含數個 LAN 的大樓，抑或是足以夠一個園區的數棟大樓，因為每個使用者均需存取中央的資訊，因此具有高速骨幹的 LAN 以及充滿大型主機和應用程式伺服器的集中式資料中心。

* 分公司

這些群組內的工作使用者人數較少，使用者間以 LAN 互聯，而存取總公司資料則透過 WAN，對於總公司資訊的存取頻率，決定了 WAN 的連線方式透過撥接還是固定專線（這些透過電信公司機房，例如兩萬元的自建 VPN 專線或約莫十三萬的點對點專線）。

/* 分公司不使用軟體 VPN 是基於流量和效能，故與電信公司申請固定專線的 VPN 。*/


* 電訊通勤者

在遠端工作者（通常是家中），需要一個即時連線（軟體 VPN），以存取總公司與分公司的資源（公司內部也要有可作相應設定的路由器或是防火牆）。

* 行動用戶

這些人往往在非固定地點工作，以撥接方式連線回總公司或是分公司，連上該處的區域網路！在公司時，工作者連上 LAN，外出時則透過撥接連上公司。

按企業需求劃分網路階層（三層式架構）：

* Core (多層交換器)
亦稱為核心層或是骨幹層，能將需求以最快速度轉成相應服務。

常見的核心服務包括寄信、會議、網際網路連線等。

* Distribution (路由器)
亦稱為分散層，處理轉送與傳送路徑，服務工作群組，路由繞送、防火牆過濾、存取廣域網路。

1. 此層將網路畫分為多個群組/廣播層。
2. 負責不同網路的資料轉換。
3. 提供封包過濾。
4. 此層為存取層的設備集結點。
5. 繞送各群組資源的網路流量。
6. 決定了交換層如何或能否存取核心層資料。

* Access (交換器)
亦稱為桌面層或是存取層，終端進入網路的入口點。

是一般使用者連上網路的入口，大多數資料均可從此層級（近處）取得，因為存取這些資源導致網路資料流量在儲存處、交換器、使用者間往返，故多個使用者群組與他們各自所屬的資源也位於這層。

然而此近處所取得的服務，通常不包含資料庫檔案等資訊，要透過分散層來提供。





