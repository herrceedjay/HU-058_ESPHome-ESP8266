# ESPHome firmware

| ESP8266(NodeMCUV2) | Pin | Net |
| --- | --- | --- |
| GPIO05(D1) | 14 on HU-058D; 16 on HU-058 / HU-058SE | CLK, driver 1 |
| GPIO04(D2) | 5 | DATA, driver 1 |
| GPIO14(D5) | 1 | CLK_1, driver 2 |
| GPIO12(D6) | 2 | DATA_1, driver 2 |
| GPIO13(D7) | 9 | S1, top button |
| GPIO3(RX) | 10 | S2, bottom button |
| GND | 8 | GND |

## Configuration

```yaml
aip33628:
  id: panel
  clk_pin: GPIO05
  data_pin: GPIO04
  clk2_pin: GPIO14
  data2_pin: GPIO12
  time_id: ha_time
  twelve_hour: true
  blink_colon: true
  max_current: 15
```


