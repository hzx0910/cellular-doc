## CSV SAMPLE

### POST Headers

    Content-Type:text/plain
    X-Client-Type:Android
    VERSION-NAME:6.x.x
    CELL-VIP-ID:xxxxxxxx
    SLOT-INDEX:1  (1 OR 2)
    OPERATOR:xxxxx  (MCC+MNC 46000\46001...)
    UUID:xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx (UNIQUE FILE ID)

### Body raw

    "TIME","LATITUDE","LONGITUDE","TYPE","NR-TAC","NR-PCI","NR-CI","NR-ARFCN","CSI-RSRP","CSI-RSRQ","CSI-SINR","SS-RSRP","SS-RSRQ","SS-SINR","TAC","PCI","ECI","EARFCN","BAND_WIDTH","RSSI","RSRP","RSRQ","SINR","CQI","LAC","CI","RXLEV","ARFCN","BSIC","PSC","UARFCN","NID","BID","SID","CDMADBM","CDMAECIO","EVDODBM","EVDOECIO","EVDOSNR"
    "20220721 10:19:00.516","40.100206","116.310889","NR","2097262","690","5744431108","504990","","","","-65","-11","23","","","","","","","","","","","2097262","","","","","0","","","","","","","","",""
    "20220721 10:19:00.640","40.100206","116.310889","NR","2097262","690","5744431108","504990","","","","-65","-11","23","","","","","","","","","","","2097262","","","","","0","","","","","","","","",""
    "20220721 10:19:00.649","40.100206","116.310889","NR","2097262","690","5744431108","504990","","","","-65","-11","23","","","","","","","","","","","2097262","","","","","0","","","","","","","","",""
    "20220721 10:19:00.697","40.100206","116.310889","NR","2097262","690","5744431108","504990","","","","-69","-11","","","","","","","","","","","","2097262","","","","","0","","","","","","","","",""
    "20220721 10:19:00.700","40.100206","116.310889","NR","2097262","690","5744431108","504990","","","","-69","-11","","","","","","","","","","","","2097262","","","","","0","","","","","","","","",""

### Body = TIME + LOCATION + CELL

#### LOCATION

    LATITUDE float
    LONGITUDE float

#### CELL COLUMNS

    TYPE,
    NR-TAC,NR-PCI,NR-CI,NR-ARFCN,
    CSI-RSRP,CSI-RSRQ,CSI-SINR,SS-RSRP,SS-RSRQ,SS-SINR,
    TAC,PCI,ECI,EARFCN,BAND_WIDTH,RSSI,RSRP,RSRQ,SINR,CQI,
    LAC,CI,RXLEV,ARFCN,BSIC,PSC,UARFCN,
    NID,BID,SID,CDMADBM,CDMAECIO,EVDODBM,EVDOECIO,EVDOSNR