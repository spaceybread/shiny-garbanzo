# Arktika 

## Geographical Considerations

From this [tweet](https://x.com/sq7ro/status/1765054741006946456), the beam is narrow and 'directed' towards Moscow. Additionally, [Arved Viehweger](https://github.com/arvedviehweger) has been recieving data from Arktika and they appear to based in Wismar, Germany. For M2 in particlar, it appears [Scott Tilley](https://x.com/coastal8049) has been able to recieve [data](https://x.com/coastal8049/status/1748927210441068819/photo/1) and they're based in Roberts Creek, Canada. Finally, Twitter user [supertrack](https://x.com/supertrack_it) seems to be able to recieve [data](https://x.com/supertrack_it/status/1477750254980190220/photo/1) from Arktika-M1. I don't know where exactly this user is based but it appears to be somewhere in Italy.  
- ROSCOSMOS: Moscow 55°45′21″N 37°37′2″E
- Arved: Wismar 53°54′N 11°28′E
- Scott: Roberts Creek 49.42397°N 123.64795°W (Wikipedia is weirdly inconsistent on the lat/lon format)
- supertrack: Roughly in Italy, confined by the 4 following points on the Earth: 
    - Northernmost point: 47°5′N 12°11′E
    - Southernmost point: 37°56′N 16°3′E
    - Westernmost point: 45°6′N 6°37′E
    - Easternmost point: 40°6′N 18°31′E
- SSEC: Madison 43°04′29″N 89°23′03″W

While I can't be certain, I believe the SSEC's (and by extension, the antenna's) location should not cause problems in attempting to recieve data from Arktika.  

## Arved's setup 

From this [article](https://www.rtl-sdr.com/receiving-x-band-images-from-the-arktika-m1-arctic-monitoring-satellite/). Connected to Arktika-M1's X-band downlink at 7865 MHz and this appears to be the only way to recieve imagery at the moment. Notably, this means having access to X-Band RF gear: 
- Low noise pre-amplifier 
- Downconverter 
- A high bandwidth SDR
Arved's equipment: 
- A pre-amp by MITEQ (36dB gain, 1dB noise figure)
- DK5AV compact X-Band downconverter (they made this themselves)
- LimeSDR-USB

He uses a Channel Master 2.4m prime focus dish in North Eastern Geramny and it produces around 9-10dB of SNR (signal to noise ratio) through SatDump. He also notes that an SNR > 5dB should have a decode but there is no forward error correction so decode does not automatically imply a clean image. 
