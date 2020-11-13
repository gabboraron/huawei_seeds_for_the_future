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

## Cloud computing
https://www.huaweicloud.com/en-us/product/
> examples: 
> - cloud sincronization
> - 5 advantages:
>   - on demand self service
>   - broad network access
>  -  resource pooling: wenever a part is broken a good one can restore it
>  - rapid elasticity
> - measured service
>
> *Reason to use cloud computing is because of the strong scalability of Cloud Computing. Also the measured service. Measurement is the unit's unification. The service can measure what we need and set that resources what we need.*

> **Cloud computing definition: resources can be quickly provisioned and released reflecting of characteristics and managing cloud computing. Generally cloud computing = internet + computing. **
>
> without computing and leaving the internet it cannot be admitted as true cloud computing 
>
> ![hitsory of internet](https://cloudcomputing521.files.wordpress.com/2017/05/the-history-of-the-cloud-1024x511.png)
>
> BT download
>
> cloud computing: 
> - cloud 1.0: computing virtualization, hyper-v
> - cloud 2.0: software definite integration: VMware, AWS - cloud based infrastructure
> - cloud 3.0: cloud native, app redesign: Docker, CoreOS, CloudFoundry - cloud native applications
>
> cloud deployment models:
> - public cloud:
>   - private cloud
>   - private clouds ensure private security
> - transportation cloud
> - financial cloud
> - heltchare cloud
>
> ![cloud service models](https://res.cloudinary.com/practicaldev/image/fetch/s--ol7OnjXd--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/flzshxgpfmu59dhor6mt.png)
>
> Paas: continued on underline resources: 
> Iaas: CPU + memory+ storage
> SaaS: all things managed by provider, example facial reognition

**Fields related to cloud computing:**
> - IoT: this is a result of the internet which connects all things. 
>   - RFID: pass card
>   - Sensors: stat information, ex: a smoke sensor that triggers fire, which opens the corridor.
>  - Embedded systems: not only need identification but also get some data, and process or preprocess that data. We collect these data for analysis and find the information we need. Human-machine connection.
>
> 4 characteristics of big data :
> - volume: the amount of data
> - velocity: the speed at which data is generated
> - variety: the different types of data
> value: the value the can be extracted from data
>
> we send the data to a place unified to process
> 1. first step is to collect the data 
> 2. parts of AI:
> 2.1 Big Data
> 2.2 Algorithm
> 2.3 Computing power
> 2.4 Scenario
> 
> **Container:**
> 
> virtualization technology
> Several containers can be created on each operating system, each of which is allocated only a subset of the computer's resources
> - Docker: open-source application container engine. It allows developer to pack their app nad dependency pack into  a portable container, and later run them on any other Linux machine.
> ![docker infographic](https://www.edureka.co/blog/wp-content/uploads/2016/10/Docker-Client-What-Is-Docker-Container-Edureka.png)
> ![differences between containers and VM](https://livecodestream.dev/amp/post/2020-06-25-intro-to-docker-for-web-developers/docker_hu26f1f4e09abb26d0091452b6c8f18010_29453_700x0_resize_q75_box.jpg)
> ![diff2](https://akfpartners.com//uploads/blog/VM_Image.PNG)
> - open stack launched by NASA, open stack is a cloud computing OS
>   - ![open stac components](https://4.bp.blogspot.com/-TAimP7yHqC4/UZ5KmCryEJI/AAAAAAAAGXY/JIBLhQ8D9R0/s1600/OpenStack_Components.png)
> 
> **Fog computing**:
>
> An extension of cloud computing services to the edge of the network to decrease latency and network congestion. Fog computing uses edge devices to carry out a substantial amount of computation, storage, and communication locally, instead of storing all data in a  cloud data centers.
> ![fog computing](https://www.itprc.com/wp-content/uploads/2018/09/Fog-Computing-diagram.jpg)
>
> **Edge computing**
>
> ![edge computing](https://cdn-images-1.medium.com/max/1024/1*sOOdwM13CQHJbuuC6QhBgA.png)

**Virtualization**
- SPECvirt:
  - virtualization performance of a single CPU
- virtualization storage:
  - SDS: consolidates the local storage used by computing nodes
    - the I/O between local and network storage is optimized to reduce latency
- network virtualization:
   - virtual machine device queues or VMDQ
   - SR-IOV
Available functions :
- reused resources
- resource pool management
- distributed power management
- distributed resources scheduling (DRS)
- storage DRS 
- deploy multiple hosts on different clusters
- VM's created manually or directly
- Cloud's HA functions rescue a shut downed VM and restart it.
- DPM: distributed power management

## AI Advanced
the learning g algorithm: is to train to catch labels nad targets, normally we used super 
- supervised algorithms
  - classification task
  - regression task
-unsupervised algorithms
  - clustering task
  - dimension deduction
- semi-supervised
 
typical machine learning process:
 - break down the problem locating data
- clean data
- select features
- Neuron: is the unit of neural network, consisting of a linear function and an activation function
  - linear function: if the input is the n dimensional feature vector , the calculation formula is as follows: `f(X,W,b) = WX + b`
- Frank- Rosenblatt perceptron: receiving multiple signals
  - good for separating things, planes, hyperplanes
  - single layer perceptron cannot solve XOR
