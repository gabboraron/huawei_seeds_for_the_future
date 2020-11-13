# huawei seeds for the future

## Cultural programs:
### painting
![chinese rooster](https://i.pinimg.com/originals/24/8c/a6/248ca6d2621b62f9d7a37f728d363fe1.jpg)
There is allways a host and a guest on a paint, a yan and a yin, here rooster is host, the writing is the guest

## HMS Core
- https://developer.huawei.com/consumer/en/hms/
- hms kit/services: https://developer.huawei.com/consumer/en/doc/10123#h1-1593324927473-3
  -  scan kit: https://developer.huawei.com/consumer/en/hms/huawei-scankit/
  
### $1 billion plan
https://cntechpost.com/2020/02/24/huawei-launches-1-billion-plan-to-encourage-developers-to-join-hms/

## AI basic
- https://forum.huawei.com/enterprise/en/introduction-to-the-machine-learning-school/thread/568685-100429
- https://en.wikipedia.org/wiki/Multilayer_perceptron

## 5G basic
- 3G https://en.wikipedia.org/wiki/3G
  - 70 min to download 80 gb at 14Mbps 
- 4G 
  - 7 min to download 80 gb at 150 Mbps
  - VR
    - 2Gbps needed
  - IoT
    - 1000 connection per cell, and increasing
- 4G-4.5G https://halberdbastion.com/technology/cellular/4g-lte/lte-evolutions
  - high latency
- 5G 
  - low latency  (1 ms)
  - 2015 in switerland
  - end to end ecosystem
  - 3 types makes one future IMT:
     - enhanced mobile broadband - eMBB
     - massive machine-type communications - MMTC
     - ultra reliable and low latency communications - uRLLC
> ITU raising new requirements, testing new technologies, develop coresponding products, deploying networks
>
> ITU and 3GPP develop the 5G standards
>
> - rel15- eMBB - 1Gbps
> - mMTC - 1Mn connections/km2
> - uRLOC - 1ms end-to-end

- Verizon 5G FWA Home, 300Mbmps
- FWA: fixed wireless Access
- eLTE: Evolved LTE
- NR: New Radio
- GSA: Global mobile supplieres Association

**LTE:**
- W-CDMA: https://www.3gpp.org/technologies/keywords-acronyms/104-w-cdma
- LTE - LTE-A - LTE-TDD: https://www.cablefree.net/wirelesstechnology/4glte/overview-of-lte-3gpp-releases/

**5G spectrum planning:**
> Shannon theory: `C=B*log2(1+S/N)`; `C`-date rate, `B`-carrier bandwith, `S/N`-signal to noise ratio (snr)
> - `B` - boost the user and technologies to reduce latency
>
> **usually mobile networks**
>
> using TDD, uplink and downlink data are transmitted on the same frequency
> 
> **5G network**
>
> 5G new radio base stations (gNodeB), use high freq to communications and low LTE freq for uplink communikations
> - if UE is close to base station, than there downlink signals are carried on the high freq band
> - when UE is far from base uplink is on low freq, but down link is on high freq band
- FR1 - sub 6GHz, 3.5 GHz - 5G main |45-6000MHz 
- FR2 - mmWave, 28/39/60/73GHz as primary bands |24250-52600MHz

- sub 3 GHz - basic covarage
- C-band - wide covarage in urban areas
- mmWave - capacity boost in hotspots
- SNR - signal to noise radio
- FR - frequnecy range

- reduce latency
- incrase the nnumber of connections
- enhance 5 coverage

coverage enhancement tecnology
rate improvement technology
latency reduction technology

**Data rate**
> 5G using massive MIMO technology and new channel coding technologies
> 
> **channel coding**
> - in addition of useful bits redundand bits are added to protect useful infomration bits, andand improve reliability of infomration transmission
> - 3GPP release 15 in 5G eMBB scenario the contorl channels use Polar codes, the traffic chanel use low density parity check (LDPC) having many advantages over the 4G Turbo coding tech
> | -                         | Turbo         | LDPC   |
> | ------------------------- |:-------------:| ------:|
> | decoding performance      | 30%           | 90%    |
> | decoing latency           | 1             |   1/3  |
> | Chip size                 | 1             |    1/3 |
> | Decoding power consumption| 1             |    1/3 |
> 
> - polar technology results in a lower error rate in data transmission when compered with Turbo tech under the same signal noise
> 
> **Massive MIMO**
> - large scale antennas with least 16 antennas 
> - with 64 antennas to achieve 64T64R
> - with large scale antenan ray solution improves coverage capability and system capacity reducing interference
> comparing massive mimo cmpared with the 8T8R antennas in 4G TDD system massive MIMO wins, 8T8R can only transmit two downlink data streams while 64T64R massive MIMO with narrower beams can provide 16 data streams in the downlink, configured with two antennas 1T2R by default, 5G UE configured with 4 antennas 2T4R
> - 8T8R sonly support horiontal beamforming after beamforming, so high residentials do not have signal, massive MIMO can make a difference 
>
> **Grant-free scheduling**
> - normally a phone sent syn-ack before data, but this send firstly uRLLC data
> - this will be frozten in release 16
> - only used in latency sensitive uRLLC scenarios
> 
> **D2D - device to device**
> - advantages: 
>   - long transmission distance ~ 1km
>   - low transmission latency
>   - high spectral effenciency
>
> **MEC - Mobile edge computing**
> - `complete latency = air transmission latency + terrestrial interface latency + device processing latency`
> - reducing `teresrial latnecy` - hierarchical core networks using edge data centers (DC) => regional DC => core DC deployed on different locations
> - for vehice to everything (V2X) and Internet of Vehicle (IoV) services core ntewrok can be deployed on edge DC, whitch maybe is on houndreds of km

**cloudification of core network**
> Next gen core => network functions virtualization
> NG-C & NG-U => soft defined networking
> gNodeB => Cloud Ran
> new-radio
>
> Arhitecture characteristic 1: **NFV**
> -*Traditional*:
>   - hardware
>      - EPC
>      - IMS
>   - software:
>     - locked in specific hardware, cmplicated capacity expansion
> -*5G*
>  - agile rollout
> 
> Arhitecture characteristic 2: **Control and User Plane Separation - CUPS**
> - *Traditional core network*
>   - user plane and CP not completly separated
>   - 4G: MME serving service gateway (SGW) or packet data network gatewey P-GW
> - *5G* - as before said
>
> Arhitecture characteristic 1: **Service Based Architecture (SBA)**
> - modular functions - costumized functions
> - not everybody needs everything
>
> **SDN**: Enlightenment of the IT industry
- Enlightment of PCs/servers
  - application program
  - operating system
  - universal PC hardware
- ever-changeing smartphones
  - open application software
  - iOS/Android
  - Smartphone hardware
- potential canges of transport networks (SDN)
  - application
  - SDN controller
  - forwarder
  - makes possible creating different networks based on different QoS
- radio access network architecture (cloud RAN)
  - age of claudification
  - baseband unit BBU deployed at wireless site  
    - gNodeB-CU ->data center NRT functions
    - gNode-DU -> wireless site RT functions
- end-to-end network sliceing
  - software defined network slicing
  - SDN/NFV

-**non-standalon network**: 5G network cannot be deployed without 4G network
-**standalone network**: does not require a 4G network 
  - next gen core network (NGC)
  - NGC signaling sent directly to gNodeB
- typical NSA network:
  - the core is NGC, the wieless is NR
  - dinamically distributed traffic

![5g evolution](https://raw.githubusercontent.com/gabboraron/huawei_seeds_for_the_future/main/5gevolution.jpg)

