<h1>My Project<h1/>
RiftBoard is a comprehensive devboard built around the RP2040 chipset, it features a very fancy (and time consuming) ground fill, some 3v3 and some VBUS, also lots of GND. I built it mainly for testing and using sensors and actuators, either on their own or working together.
<h1>Why?</h1>
I started this project because I wanted to get into hardware design and embedded electronics. But also because I love HackClub and what they do and really wanted to be a part of this, I thank you so much for the opportunities, and I also really want a hot plate for future projects :).

<h1>Pics<h1/>
<img width="589" height="403" alt="image" src="https://github.com/user-attachments/assets/69c692a6-f992-43b9-9327-5bf30410a61b" />
<img width="133" height="312" alt="image" src="https://github.com/user-attachments/assets/f4f183dc-f220-4d35-b5ad-534a5e3fd66f" />
<img width="1722" height="977" alt="RiftBoard" src="https://github.com/user-attachments/assets/8b257af1-c0a9-45e9-a17f-89f33f6e4f6c" />
<img width="1722" height="977" alt="RiftBoardBack" src="https://github.com/user-attachments/assets/05101d70-67d9-4b88-8cf7-44c0ef374feb" />

<h1>BOM</h1>
<table>
    <tr>
        <td>Mrf#</td>
        <td>Mfr.</td>
        <td>Order Qty.</td>
        <td>Unit Price(USD)</td>
        <td>Ext.Price(USD)</td>
        <td>LCSC#</td>
        <td>Package</td>
        <td>Min</td>
        <td>Mult</td>
        <td>SPQ</td>
        <td>Availability</td>
        <td>Stock Status</td>
        <td>Customer Notes</td>
        <td>Description</td>
        <td>Purpose</td>
        <td>Product Link</td>
    </tr>
    <tr>
        <td>CC0402KRX7R7BB104</td>
        <td>YAGEO</td>
        <td>100</td>
        <td>0.0010</td>
        <td>0.10</td>
        <td>C60474</td>
        <td>0402</td>
        <td>100</td>
        <td>100</td>
        <td>10000</td>
        <td>11898300</td>
        <td>In Stock</td>
        <td></td>
        <td>100nF ±10% 16V Ceramic Capacitor X7R 0402</td>
        <td>Capacitors for decoupling and stabilisation of powerlines</td>
        <td>https://www.lcsc.com/product-detail/C60474.html</td>
    </tr>
    <tr>
        <td>CL05A105KP5NNNC</td>
        <td>Samsung Electro-Mechanics</td>
        <td>100</td>
        <td>0.0023</td>
        <td>0.23</td>
        <td>C14445</td>
        <td>0402</td>
        <td>100</td>
        <td>100</td>
        <td>10000</td>
        <td>1500800</td>
        <td>In Stock</td>
        <td></td>
        <td>1uF ±10% 10V Ceramic Capacitor X5R 0402</td>
        <td>One for each power line</td>
        <td>https://www.lcsc.com/product-detail/C14445.html</td>
    </tr>
    <tr>
        <td>CL10A106KP8NNNC</td>
        <td>Samsung Electro-Mechanics</td>
        <td>50</td>
        <td>0.0080</td>
        <td>0.40</td>
        <td>C19702</td>
        <td>0603</td>
        <td>50</td>
        <td>50</td>
        <td>4000</td>
        <td>3665250</td>
        <td>In Stock</td>
        <td></td>
        <td>10uF ±10% 10V Ceramic Capacitor X5R 0603</td>
        <td>Caps for the stepdown converter</td>
        <td>https://www.lcsc.com/product-detail/C19702.html</td>
    </tr>
    <tr>
        <td>CL05C330JB5NNNC</td>
        <td>Samsung Electro-Mechanics</td>
        <td>100</td>
        <td>0.0036</td>
        <td>0.36</td>
        <td>C70465</td>
        <td>0402</td>
        <td>100</td>
        <td>100</td>
        <td>10000</td>
        <td>209500</td>
        <td>In Stock</td>
        <td></td>
        <td>33pF ±5% 50V Ceramic Capacitor C0G 0402</td>
        <td>Caps for the crystal</td>
        <td>https://www.lcsc.com/product-detail/C70465.html</td>
    </tr>
    <tr>
        <td>YLED0603B</td>
        <td>YONGYUTAI</td>
        <td>100</td>
        <td>0.0060</td>
        <td>0.60</td>
        <td>C19171394</td>
        <td>0603</td>
        <td>100</td>
        <td>100</td>
        <td>4000</td>
        <td>55000</td>
        <td>In Stock</td>
        <td></td>
        <td>Blue LED Indication - Discrete 2.6V~3.2V 0603</td>
        <td>Blue programmable LED</td>
        <td>https://www.lcsc.com/product-detail/C19171394.html</td>
    </tr>
    <tr>
        <td>YLED0603R</td>
        <td>YONGYUTAI</td>
        <td>100</td>
        <td>0.0061</td>
        <td>0.61</td>
        <td>C19171390</td>
        <td>0603</td>
        <td>100</td>
        <td>100</td>
        <td>4000</td>
        <td>267100</td>
        <td>In Stock</td>
        <td></td>
        <td>Red LED Indication - Discrete 1.8V~2.4V 0603</td>
        <td>Red programmable LED</td>
        <td>https://www.lcsc.com/product-detail/C19171390.html</td>
    </tr>
    <tr>
        <td>HX TYPE-C 16PIN</td>
        <td>hanxia</td>
        <td>5</td>
        <td>0.0704</td>
        <td>0.35</td>
        <td>C5178539</td>
        <td>SMD</td>
        <td>5</td>
        <td>5</td>
        <td>1000</td>
        <td>34690</td>
        <td>In Stock</td>
        <td></td>
        <td>USB-C (USB TYPE-C) Receptacle Connector 16 Position Surface Mount, Right Angle</td>
        <td>Usb interface</td>
        <td>https://www.lcsc.com/product-detail/C5178539.html</td>
    </tr>
    <tr>
        <td>PH2.54-1X20P-H25</td>
        <td>JXTCONN</td>
        <td>10</td>
        <td>0.0920</td>
        <td>0.92</td>
        <td>C42431804</td>
        <td>Through Hole,P=2.54mm</td>
        <td>5</td>
        <td>5</td>
        <td>200</td>
        <td>9870</td>
        <td>In Stock</td>
        <td></td>
        <td>Pin Header 20 Position 2.54mm Pitch Single Row Through Hole -40℃~+105℃</td>
        <td>Main Pin headers</td>
        <td>https://www.lcsc.com/product-detail/C42431804.html</td>
    </tr>
    <tr>
        <td>HX PH254-01-03-Z-L11.5 pcb pin header</td>
        <td>hanxia</td>
        <td>20</td>
        <td>0.0192</td>
        <td>0.38</td>
        <td>C52016391</td>
        <td>Through Hole,P=2.54mm</td>
        <td>20</td>
        <td>20</td>
        <td>2000</td>
        <td>9760</td>
        <td>In Stock</td>
        <td></td>
        <td>Pin Header 1 2.5mm 6mm 3P -40℃~+105℃ 3mm 2.54mm 3A 1kV 1x3P Through Hole,P=2.54mm Headers, Male Pins RoHS</td>
        <td>3pin-connector</td>
        <td>https://www.lcsc.com/product-detail/C52016391.html</td>
    </tr>
    <tr>
        <td>RC0402FR-075K1L</td>
        <td>YAGEO</td>
        <td>100</td>
        <td>0.0009</td>
        <td>0.09</td>
        <td>C105872</td>
        <td>0402</td>
        <td>100</td>
        <td>100</td>
        <td>10000</td>
        <td>1024700</td>
        <td>In Stock</td>
        <td></td>
        <td>5.1kΩ 62.5mW 50V Thick Film Resistor ±100ppm/℃ ±1% 0402 Chip Resistor - Surface Mount RoHS</td>
        <td>Pull-down resistors for CC1/2 on usb interface</td>
        <td>https://www.lcsc.com/product-detail/C105872.html</td>
    </tr>
    <tr>
        <td>FRC0402F27R0TS</td>
        <td>FOJAN</td>
        <td>100</td>
        <td>0.0006</td>
        <td>0.06</td>
        <td>C2909343</td>
        <td>0402</td>
        <td>100</td>
        <td>100</td>
        <td>10000</td>
        <td>443300</td>
        <td>In Stock</td>
        <td></td>
        <td>27Ω ±1% 62.5mW 0402 Thick Film Resistor</td>
        <td>Resistors for the differential pair to usb interface</td>
        <td>https://www.lcsc.com/product-detail/C2909343.html</td>
    </tr>
    <tr>
        <td>RC0402FR-071KL</td>
        <td>YAGEO</td>
        <td>100</td>
        <td>0.0008</td>
        <td>0.08</td>
        <td>C106235</td>
        <td>0402</td>
        <td>100</td>
        <td>100</td>
        <td>10000</td>
        <td>5051800</td>
        <td>In Stock</td>
        <td></td>
        <td>1kΩ 62.5mW 50V Thick Film Resistor ±100ppm/℃ ±1% 0402 Chip Resistor - Surface Mount RoHS</td>
        <td>One for the crystal and one for flash mem</td>
        <td>https://www.lcsc.com/product-detail/C106235.html</td>
    </tr>
    <tr>
        <td>RC0402FR-0710KL</td>
        <td>YAGEO</td>
        <td>100</td>
        <td>0.0008</td>
        <td>0.08</td>
        <td>C60490</td>
        <td>0402</td>
        <td>100</td>
        <td>100</td>
        <td>10000</td>
        <td>1433400</td>
        <td>In Stock</td>
        <td></td>
        <td>62.5mW 10kΩ 50V Thick Film Resistor ±100ppm/℃ ±1% 0402 Chip Resistor - Surface Mount RoHS</td>
        <td>Flash mem to power resistor</td>
        <td>https://www.lcsc.com/product-detail/C60490.html</td>
    </tr>
    <tr>
        <td>FRC0402F50R0TS</td>
        <td>FOJAN</td>
        <td>100</td>
        <td>0.0006</td>
        <td>0.06</td>
        <td>C51048227</td>
        <td>0402</td>
        <td>100</td>
        <td>100</td>
        <td>10000</td>
        <td>495800</td>
        <td>In Stock</td>
        <td></td>
        <td>62.5mW 50Ω 50V Thick Film Resistor ±100ppm/℃ ±1% 0402 Chip Resistor - Surface Mount RoHS</td>
        <td>50R resistor for Red LED</td>
        <td>https://www.lcsc.com/product-detail/C51048227.html</td>
    </tr>
    <tr>
        <td>0603WAF100JT5E</td>
        <td>UNI-ROYAL</td>
        <td>20</td>
        <td>0.0017</td>
        <td>0.03</td>
        <td>C22859</td>
        <td>0603</td>
        <td>20</td>
        <td>20</td>
        <td>5000</td>
        <td>158680</td>
        <td>In Stock</td>
        <td></td>
        <td>10Ω ±1% 100mW 0603 Thick Film Resistor</td>
        <td>10R resistor for Blue LED</td>
        <td>https://www.lcsc.com/product-detail/C22859.html</td>
    </tr>
    <tr>
        <td>TS-1088-AR02016</td>
        <td>XUNPU</td>
        <td>10</td>
        <td>0.0545</td>
        <td>0.55</td>
        <td>C720477</td>
        <td>SMD,4x3mm</td>
        <td>10</td>
        <td>10</td>
        <td>4000</td>
        <td>376970</td>
        <td>In Stock</td>
        <td></td>
        <td>Tactile Switch SPST 160gf 2mm SMD (SMT) Tab 4mm x 3mm Surface Mount</td>
        <td>One switch for flash write mode, and one programmable.</td>
        <td>https://www.lcsc.com/product-detail/C720477.html</td>
    </tr>
    <tr>
        <td>RP2040</td>
        <td>Raspberry Pi</td>
        <td>5</td>
        <td>0.9482</td>
        <td>4.74</td>
        <td>C2040</td>
        <td>LQFN-56(7x7)</td>
        <td>1</td>
        <td>1</td>
        <td>3400</td>
        <td>101373</td>
        <td>In Stock</td>
        <td></td>
        <td>133MHz 30 LQFN-56(7x7) Microcontrollers RoHS</td>
        <td>The MCU on this board</td>
        <td>https://www.lcsc.com/product-detail/C2040.html</td>
    </tr>
    <tr>
        <td>MCP1700T-3302E/TT</td>
        <td>MICROCHIP</td>
        <td>5</td>
        <td>0.3762</td>
        <td>1.88</td>
        <td>C39051</td>
        <td>SOT-23</td>
        <td>5</td>
        <td>5</td>
        <td>3000</td>
        <td>9370</td>
        <td>In Stock</td>
        <td></td>
        <td>3.3V Positive Fixed SOT-23 Voltage Regulators - Linear, Low Drop Out (LDO) Regulators RoHS</td>
        <td>The stepdown converter from 5v to 3v3</td>
        <td>https://www.lcsc.com/product-detail/C39051.html</td>
    </tr>
    <tr>
        <td>W25Q16JVUXIQ</td>
        <td>Winbond</td>
        <td>10</td>
        <td>1.0529</td>
        <td>10.53</td>
        <td>C2843335</td>
        <td>USON-8-EP(2x3)</td>
        <td>10</td>
        <td>10</td>
        <td>4000</td>
        <td>34380</td>
        <td>In Stock</td>
        <td></td>
        <td>2.7V~3.6V 16Mbit 133MHz SPI USON-8-EP(2x3) Memory (ICs) RoHS</td>
        <td>The flash memory module</td>
        <td>https://www.lcsc.com/product-detail/C2843335.html</td>
    </tr>
    <tr>
        <td>X322512MSB4SI</td>
        <td>YXC Crystal Oscillators</td>
        <td>10</td>
        <td>0.0734</td>
        <td>0.73</td>
        <td>C9002</td>
        <td>SMD3225-4P</td>
        <td>10</td>
        <td>10</td>
        <td>3000</td>
        <td>436800</td>
        <td>In Stock</td>
        <td></td>
        <td>Crystal 12MHz ±10ppm 20pF SMD3225-4P</td>
        <td>the Crystal oscilator</td>
        <td>https://www.lcsc.com/product-detail/C9002.html</td>
    </tr>
</table>
