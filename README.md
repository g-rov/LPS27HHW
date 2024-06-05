# LPS27HHW
Arduino library for STMicroelectronics LPS27HHW absolute barometer

- Included set/get function for Ouput Data Rate (ODR) and Low Pass filter bandwidth (LP).

## Constructors

LPS22HHSensor(TwoWire *i2c, uint8_t address);

LPS22HHSensor(SPIClass *spi, int cs_pin, uint32_t spi_speed);

## Functions 

begin();

end();

ReadID(uint8_t *Id);

Enable();

Disable();

GetOutputDataRate(float *Odr);

SetOutputDataRate(float Odr);

GetLPBandwidth(float *Lp);

SetLPBandwidth(float Lp);

GetPressure(float *Value);

Get_PRESS_DRDY_Status(uint8_t *Status);

GetTemperature(float *Value);

Get_TEMP_DRDY_Status(uint8_t *Status);

Read_Reg(uint8_t reg, uint8_t *Data);

Write_Reg(uint8_t reg, uint8_t Data);

Get_FIFO_Data(float *Press, float *Temp);

Get_FIFO_FTh_Status(uint8_t *Status);

Get_FIFO_Full_Status(uint8_t *Status);

Get_FIFO_Ovr_Status(uint8_t *Status);

Get_FIFO_Level(uint8_t *Status);

Reset_FIFO_Interrupt(uint8_t interrupt);

Set_FIFO_Interrupt(uint8_t interrupt);

Set_FIFO_Mode(uint8_t Mode);

Set_FIFO_Watermark_Level(uint8_t Watermark);

Stop_FIFO_On_Watermark(uint8_t Stop);

Set_One_Shot();

Get_One_Shot_Status(uint8_t *Status);
