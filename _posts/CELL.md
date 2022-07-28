## CELL SAMPLE

### Type

    NR | LTE | GSM | WCDMA | TDSCDMA | CDMA | NONE

### NR (New Radio) 

    int   nr_tac ;  //16-bit Tracking Area Code 追踪区域码
    int   nr_pci ;  //0..1007 Physical Cell Identifier 物理小区标识
    long  nci ;     //[0, 68719476735] Cell Identifier 小区标识
    int   nrarfcn ; //[0, 3279165] Absolute Radio Frequency Channel Number 绝对无线频道编号

    int   csi_rsrp ; //Range: -140 dBm to -44 dBm.
    int   csi_rsrq ; //Range: -20 dB to -3 dB.
    int   csi_sinr ; //Range: -23 dB to 23 dB
    int   ss_rsrp ;  //Range: -140 dBm to -44 dBm.
    int   ss_rsrq ;  //Range: -20 dB to -3 dB.
    int   ss_sinr ;  //Range: -23 dB to 40 dB

### LTE | NSA

    int   tac ; //16-bit Tracking Area Code
    int   pci ; //0..1007
    int   eci ; 
    int   earfcn ; 
    int   band_width ; //kHz Android 9.0+

    int   rssi ; //系统出的值是正的 -113 + 2 * SignalStrength
    int   rsrp ; 
    int   rsrq ; 
    float sinr ; //dB
    int   cqi ; 

### GSM | TD-SCDMA | WCDMA

    int   lac ; 
    int   ci ; 
    int   rxlev ; 
    int   arfcn ; 
    int   bsic ; 
    int   psc ; //wcdma only
    int   uarfcn ; //wcdma only

### CDMA

    int   nid ; 
    int   bid ; 
    int   sid ; 
    int   cdmadbm ; 
    float cdmaecio ; 
    int   evdodbm ; 
    float evdoecio ; 
    int   evdosnr ; // Valid values are 0-8.  8 is the highest signal to noise ratio