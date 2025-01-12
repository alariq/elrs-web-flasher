<template>
                <VExpansionPanels variant="popout">
                  <VExpansionPanel title="ІНФОРМАЦІЯ ПРО ПРОШИВКУ (клацни на мене):" >
                    <VExpansionPanelText>
                    <VCardTitle>General info</VCardTitle>
                    <VCardText>
                      <ul>Custom firmware supports:
                      <li>custom frequencies (who might have thought!)</li>
                      <li>switching video channels during flight easilly just with any switch on your handset (works with relay drone as well)</li>
                      <li>some non compatible changes to mitigate spoofing/hijack of the link</li>
                      </ul>
                      <br>

                      <p>
                      WiFi is not advertized, so you need to add it on your PC/phone first:<br>
                      <b>wifi</b>: ELRS RX CUSTOM / ELRS TX CUSTOM<br>
                      <b>passwd</b>: elrs_custom<br>
                      </p>

                      <p>
                      ELRS Module Hostname/IP<br>
                      <b>hostname</b>: elrs_rx_custom.local / elrs_tx_custom.local<br>
                      <b>ip</b>: 10.0.0.13<br>
                      </p>
                    </VCardText>

                    <VCardTitle>Firmware types:</VCardTitle>
                    <VCardText>
                      <ul>
                      <li><b>3.5.3-cust-freq</b> - Custom Firmware based on original ELRS 3.5.3 version. Compatible with standard ELRS</li>
                      <li><b>3.5.3-nocompat</b> - Custom Firmware based on original ELRS 3.5.3 version with additional modifications to resist spoofing/hijack. NOT compatible with standard ELRS.</li>
                      </ul>
                    </VCardText>

                    <a href="README.txt">README.txt</a> &nbsp; | &nbsp;
                    <a href="README.pdf">Налаштування</a> &nbsp; | &nbsp;
                    <a href="mailto:94df6040915a6a1e3e7485ebedd34710@proton.me">Пошта: 94df6040915a6a1e3e7485ebedd34710@proton.me</a>

                    </VExpansionPanelText>
                  </VExpansionPanel>
                </VExpansionPanels>
</template>