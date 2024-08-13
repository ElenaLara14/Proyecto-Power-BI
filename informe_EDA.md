
# Exploración de Datos: Análisis EDA
________________________________________


### 1. hotel 🏨 (Tipo de hotel)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 2
- **Valores Únicos:** Resort Hotel, City Hotel, nan
- **Tipo de Dato:** `object` OK
- **Tratamiento de Nulos:** 
  - Imputar nulos con "Desconocido".
  

### 2. is_canceled ❌ (Indica si la reserva fue cancelada)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 2
- **Valores Únicos:** False, True, nan
- **Tipo de Dato:** `object` OK
- **Tratamiento de Nulos:** 
  - Imputar nulos con "Desconocido".
  

### 3. lead_time ⏳ (Número de días entre la fecha de reserva y la fecha de llegada)
- **Nulos:** 63387 (34.66%) ⚠️
- **Unique:** 579
-- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - Imputar nulos con la mediana o media ??
  

### 4. arrival_date_year 📅 (Año de llegada al hotel)🚩🚩
- **Nulos:** 118048 (64.55%) ⚠️
- **Unique:** 3
- **Valores Únicos:** 2015.0, nan, 2016.0, 2017.0
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - fillna (0)?

### 5. arrival_date_month 📆 (Mes de llegada al hotel)🚩🚩
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 15
- **Valores Únicos:** July, August, September, October, November, etc
- **Tipo de Dato:** `object`OK
- **Transformaciones:** 
- Convertir todos los valores numéricos a nombres de meses correspondientes.
- **Tratamiento de Nulos:** 
  - Imputar nulos con "Desconocido".

### 6. arrival_date_week_number 📅 (Número de la semana de llegada al hotel)
- **Nulos:** 81873 (44.77%) ⚠️
- **Unique:** 53
- **Tipo de Dato:** `float64`
- **ELIMINAR COLUMNA**


### 7. arrival_date_day_of_month 📅 (Día del mes de llegada al hotel)
- **Nulos:** 63606 (34.78%) ⚠️
- **Unique:** 31
- **Valores Únicos:** 1.0, 2.0, nan, 3.0, 4.0, etc
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - Imputar nulos con el día más frecuente o mediana del mes o KNN

### 8. stays_in_weekend_nights 🛏️ (Número de noches durante el fin de semana)
- **Nulos:** 63387 (34.66%) ⚠️
- **Unique:** 117
- **Valores Únicos:** 0.0, 1.0, 2.0, 4.0, 3.0, etc
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - Imputar nulos con la mediana o la moda del número de noches.
  

### 9. stays_in_week_nights 🛏️ (Número de noches durante la semana)
- **Nulos:** 63387 (34.66%) ⚠️
- **Unique:** 135
- **Valores Únicos:** 0.0, 1.0, 2.0, 3.0, 4.0, etc
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - Imputar nulos con la mediana o moda del número de noches.
 

### 10. adults 👥 (Número de adultos en la reserva)🚩🚩
- **Nulos:** 63449 (34.69%) ⚠️
- **Unique:** 30
- **Valores Únicos:** 2.0, 1.0, 51.0, 3.0, 52.0, 53.0, 55.0, 57.0, 54.0, 59.0, 4.0, 58.0, 56.0, 50.0, 26.0, 27.0, 0.0, 20.0, 6.0, 5.0, 10.0, 16.0, 19.0, 11.0, 13.0, 15.0, 14.0, 12.0, 18.0, 17.0, NaN
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - Imputar nulos con la mediana o moda del número de adultos o "0"
  - Revisar valores atípicos como 51.0 y 52.0 para posible corrección antes de la imputación.

### 11. children 🧒 (Número de niños en la reserva)🚩🚩
- **Nulos:** 113575 (62.10%) ⚠️
- **Unique:** 14
- **Valores Únicos:** 0.0, 1.0, 2.0, 3.0, 10.0, 19.0, 17.0, 11.0, 18.0, 13.0, 16.0, 14.0, 15.0, 12.0, NaN
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - Imputar nulos con la mediana o moda del número de niño o "0"
  
### 12. babies 👶 (Número de bebés en la reserva)🚩🚩
- **Nulos:** 63446 (34.69%) ⚠️
- **Unique:** 14
- **Valores Únicos:** 0.0, 1.0, 18.0, 2.0, 17.0, 13.0, 15.0, 16.0, 12.0, 10.0, 11.0, 19.0, 9.0, 14.0, NaN
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - Imputar nulos con la mediana o moda del número de bebés.
  - 

### 13. meal 🍽️ (Tipo de comida incluida en la reserva)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 5
- **Valores Únicos:** 'BB', 'FB', 'HB', 'SC', 'Undefined'
- **Tipo de Dato:** `object`OK
- **Transformaciones:** Ninguna.
- **Tratamiento de Nulos:** 
- 

### 14. country 🌍 (País de origen del cliente)
- **Nulos:** 117823 (64.43%) ⚠️
- **Unique:** 163
- **Valores Únicos:** PRT, nan, GBR, USA, ESP, etc
- **Tipo de Dato:** `object`OK
- **Transformaciones:** Ninguna.
- **Tratamiento de Nulos:** 
 

### 15. market_segment 🎯 (Segmento de mercado al que pertenece la reserva)
- **Nulos:** 122943 (67.23%) ⚠️
- **Unique:** 8
- **Valores Únicos:**  'Aviation', 'Complementary', 'Corporate', 'Direct', 'Groups', 'Offline TA/TO', 'Online TA', 'Undefined'
- **Tipo de Dato:** `object`OK
- **Transformaciones:** Ninguna.
- **Tratamiento de Nulos:** 
  

### 16. distribution_channel 📢 (Canal de distribución utilizado)
- **Nulos:** 76978 (42.09%) ⚠️
- **Unique:** 5
- **Valores Únicos:** 'Corporate', 'Direct', 'GDS', 'TA/TO', 'Undefined'
- **Tipo de Dato:** `object`OK
- **Transformaciones:** Ninguna.
- **Tratamiento de Nulos:** 

### 17. is_repeated_guest 🔁 (Indica si el cliente es un huésped repetido)
- **Nulos:** 68501 (37.46%) ⚠️
- **Unique:** 2
- **Valores Únicos:** 0.0, nan, 1.0
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a booleano (`True/False`) o `int`???
- **Tratamiento de Nulos:** 
 

### 18. previous_cancellations ❌ (Número de reservas canceladas antes)
- **Nulos:** 106649 (58.32%) ⚠️
- **Unique:** 21
- **Valores Únicos:** nan, 0.0, 14.0, 10.0, 19.0, etc
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  

### 19. previous_bookings_not_canceled ✔️ (Número de reservas no canceladas)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 73
- **Valores Únicos:** 0.0, 1.0, 2.0, 3.0, 4.0, etc
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 


### 20. reserved_room_type 🛏️ (Tipo de habitación reservada)
- **Nulos:** 103602 (56.65%) ⚠️
- **Unique:** 10
- **Valores Únicos:** 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'L', 'P'
- **Tipo de Dato:** `object`OK
- **Transformaciones:** Ninguna.
- **Tratamiento de Nulos:** 
  -

### 21. assigned_room_type 🛏️ (Tipo de habitación asignada en la reserva)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 12
- **Valores Únicos:** C, A, D, E, G, F, I, B, H, P, L, K, NaN
- **Tipo de Dato:** `object`OK
- **Transformaciones:** Ninguna.
- **Tratamiento de Nulos:** 
  -

### 22. booking_changes 🔄 (Número de cambios realizados en la reserva)
- **Nulos:** 63459 (34.70%) ⚠️
- **Unique:** 22
- **Valores Únicos:** 3.0, 4.0, 0.0, 1.0, 2.0, etc
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  -

### 23. agent 🧑‍💼 (Identificador del agente involucrado)
- **Nulos:** 79827 (43.65%) ⚠️
- **Unique:** 333
- **Valores Únicos:** nan, 304.0, 240.0, 303.0, 15.0, etc
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - 

### 24. company 🏢 (Identificador de la compañía involucrada)
- **Nulos:** 179007 (97.88%) ⚠️
- **Unique:** 310
- **Valores Únicos:** nan, 110.0, 270.0, 240.0, 154.0, etc
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - **ELIMINAR COLUMNA**

### 25. days_in_waiting_list 📅 (Número de días en lista de espera)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 128
- **Valores Únicos:** 0.0, 50.0, 47.0, 65.0, 122.0, etc
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - 

### 26. customer_type 👥 (Tipo de cliente)
- **Nulos:** 88678 (48.49%) ⚠️
- **Unique:** 4
- **Valores Únicos:** Transient, nan, Contract, Transient-Party, Group
- **Tipo de Dato:** `object`OK
- **Transformaciones:** Ninguna.
- **Tratamiento de Nulos:** 
  - 

### 27. adr 💵 (Tarifa promedio diaria pagada por la reserva)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 8879
- **Valores Únicos:** 0.0, 75.0, 98.0, 107.0, 103.0, etc
- **Tipo de Dato:** `float64`OK
- **Transformaciones:** Ninguna.
- **Tratamiento de Nulos:** 
  - .

### 28. required_car_parking_spaces 🚗 (Número de espacios de estacionamiento requeridos)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 5
- **Valores Únicos:** 0.0, 1.0, 2.0, 8.0, 3.0
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - 

### 29. total_of_special_requests ✅ (Número total de solicitudes especiales)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 6
- **Valores Únicos:** 0.0, 1.0, 3.0, 2.0, 4.0
- **Tipo de Dato:** `float64`
- **Transformaciones:** 
  - Cambiar tipo de dato de `float` a `int64`.
- **Tratamiento de Nulos:** 
  - 

### 30. reservation_status 📋 (Estado de la reserva)
- **Nulos:** 63487 (34.72%) ⚠️
- **Unique:** 3
- **Valores Únicos:** Check-Out, Canceled, No-Show, nan
- **Tipo de Dato:** `object`OK
- **Transformaciones:** Ninguna.
- **Tratamiento de Nulos:** 
  - 

### 31. reservation_status_date 📅 (Fecha del estado de la reserva)
**Nulos:** 991 (0.52%) ⚠️
**Unique:** 1589
**Valores Únicos:** '2015-07-01 00:00:00', '2015-07-02 00:00:00', ..., '2027-11-31', '2024-11-31', etc
**Tipo de Dato:** object (fecha)
- **Transformaciones:** Cambiar a fecha en TABLEAU.
**Tratamiento de Nulos:** 

### 32. 0 (Columna sin nombre específico)
**Nulos:** 139926 (76.51%) ⚠️
**Unique:** 1589
**Valores Únicos:** NaN, 'City Hotel', 'True', '1/01/16', '197.1', '29/10/15', '4/02/17'
**Tipo de Dato:** object
**ELIMINAR COLUMNA**