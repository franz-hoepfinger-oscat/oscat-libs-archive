# Sheet: Vergleichstabelle

| SPS Übersicht                                                                       | Unnamed: 1    | Unnamed: 2                       | Unnamed: 3     | Unnamed: 4                        |
|:------------------------------------------------------------------------------------|:--------------|:---------------------------------|:---------------|:----------------------------------|
| nan                                                                                 | nan           | nan                              | nan            | nan                               |
| Oscat übernimmt keine Garantie auf Vollständigkeit und / oder Richtigkeit der Daten | nan           | nan                              | nan            | nan                               |
| nan                                                                                 | nan           | nan                              | nan            | nan                               |
| Hersteller                                                                          | WAGO          | Beckhoff                         | Beckhoff       | Moeller                           |
| Typ                                                                                 | 750-841       | BX9000                           | CX9001-1001    | EC4P-222                          |
| CPU                                                                                 | Strongarm     | Microcontroller                  | IXP420         | C16                               |
| Architektur                                                                         | 32 Bit        | 16 Bit                           | 32 Bit         | 16 Bit                            |
| Arithmetik Unit                                                                     | ---           | ---                              | ---            | ---                               |
| Frequenz                                                                            | nan           | nan                              | 266 Mhz        | nan                               |
| Memory Programm/Daten                                                               | 512KB / 256KB | 256KB / 256KB                    | 128MB          | 256KB / 224KB                     |
| FLASH                                                                               | 24KB          | 2KB                              | 64MB           | 1MB                               |
| File System                                                                         | 1MB           | ---                              | Ja             | MMC 64MB                          |
| RTC                                                                                 | Ja            | Ja                               | Ja             | Ja                                |
| Ethernet                                                                            | 10/100MBit    | 10/100Mbit                       | 2 * 10/100Mbit | 1 * 10Mbit                        |
| Display, Tastatur                                                                   | nan           | LCD + Tastatur                   | nan            | LCD + Tastatur                    |
| Ausgänge                                                                            | nan           | nan                              | nan            | 6 * Relais1 * AO                  |
| Eingänge                                                                            | nan           | nan                              | nan            | 12 * DI4 * AI 0-10V               |
| COMM                                                                                | ---           | 1 * RS2321 * RS232/RS4851 *  CAN | ---            | 2 * RS2321 * easy NET1 * Can open |
| Temperaturbereich [°C]                                                              | nan           | nan                              | nan            | -25 .. +55                        |
| Leistungsverbrauch [W]                                                              | 1.7           | 3.3                              | 6              | 3.4                               |
| Min Cycle Time [ms]                                                                 | 2             | 1                                | 1              | 1                                 |
| Byte Logic Test [ms]                                                                | 4.9           | 8.8                              | 0.35           | 10.1                              |
| DWORD Logic Test [ms]                                                               | 2.8           | 18                               | 0.23           | 19.5                              |
| INT Test [ms]                                                                       | 14            | 9.5                              | 1.1            | 8.81                              |
| Floating Test [ms]                                                                  | 722           | 3310                             | 143            | 338                               |
| Array_sort_test [ms]                                                                | 1.8           | 4                                | 0.32           | 4.1                               |


# Sheet: Sourcecode

| Sourcecode                 | Unnamed: 1                                                                                      | Unnamed: 2                                               |
|:---------------------------|:------------------------------------------------------------------------------------------------|:---------------------------------------------------------|
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FUNCTION_BLOCK Performance | nan                                                                                             | nan                                                      |
| VAR_INPUT                  | nan                                                                                             | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR_OUTPUT                 | nan                                                                                             | nan                                                      |
| nan                        | T_CYCLE : REAL;                                                                                 | nan                                                      |
| nan                        | T_L8 : REAL;                                                                                    | nan                                                      |
| nan                        | T_L32 : REAL;                                                                                   | nan                                                      |
| nan                        | T_INT : REAL;                                                                                   | nan                                                      |
| nan                        | T_FLOAT : REAL;                                                                                 | nan                                                      |
| nan                        | T_ARRAY : REAL;                                                                                 | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR CONSTANT               | nan                                                                                             | nan                                                      |
| nan                        | t_max : DWORD := 100000;                                                                        | nan                                                      |
| nan                        | c_max : DWORD := 10000;                                                                         | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR                        | nan                                                                                             | nan                                                      |
| nan                        | mode : INT;                                                                                     | nan                                                      |
| nan                        | start: DWORD;                                                                                   | nan                                                      |
| nan                        | cycles : DWORD;                                                                                 | nan                                                      |
| nan                        | temp8: BYTE;                                                                                    | nan                                                      |
| nan                        | temp_32: DWORD;                                                                                 | nan                                                      |
| nan                        | tx: DWORD;                                                                                      | nan                                                      |
| nan                        | TEST_ARRAY: BOOL;                                                                               | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| tx := T_PLC_US();          | nan                                                                                             | nan                                                      |
| CASE mode OF               | nan                                                                                             | nan                                                      |
| 0:                         | (* measure the execution time *)                                                                | nan                                                      |
| nan                        | cycles := 0;                                                                                    | nan                                                      |
| nan                        | mode := 1;                                                                                      | nan                                                      |
| nan                        | start := tx;                                                                                    | nan                                                      |
| 1:                         | (* perform measurement for 100ms *)                                                             | nan                                                      |
| nan                        | IF (tx - start) < 1000000 THEN                                                                  | nan                                                      |
| nan                        | nan                                                                                             | cycles := cycles + 1;                                    |
| nan                        | ELSE                                                                                            | nan                                                      |
| nan                        | nan                                                                                             | T_cycle := DWORD_TO_REAL((tx - start) / cycles)/1000000; |
| nan                        | nan                                                                                             | mode := 2;                                               |
| nan                        | END_IF;                                                                                         | nan                                                      |
| 2:                         | (* perform 8 Bit logic test *)                                                                  | nan                                                      |
| nan                        | start := tx;                                                                                    | nan                                                      |
| nan                        | cycles := 0;                                                                                    | nan                                                      |
| nan                        | REPEAT                                                                                          | nan                                                      |
| nan                        | nan                                                                                             | cycles := cycles + 1;                                    |
| nan                        | nan                                                                                             | TEST_L8();                                               |
| nan                        | UNTIL (Cycles > C_max) OR ((T_PLC_US() - start) >= t_max) END_REPEAT;                           | nan                                                      |
| nan                        | T_L8 := DWORD_TO_REAL((T_PLC_US() - start) / cycles)/1000000;                                   | nan                                                      |
| nan                        | mode := 3;                                                                                      | nan                                                      |
| 3:                         | (* perform 32 Bit logic test *)                                                                 | nan                                                      |
| nan                        | start := tx;                                                                                    | nan                                                      |
| nan                        | cycles := 0;                                                                                    | nan                                                      |
| nan                        | REPEAT                                                                                          | nan                                                      |
| nan                        | nan                                                                                             | cycles := cycles + 1;                                    |
| nan                        | nan                                                                                             | TEST_L32();                                              |
| nan                        | UNTIL (Cycles > C_max) OR ((T_PLC_US() - start) >= t_max) END_REPEAT;                           | nan                                                      |
| nan                        | T_L32 := DWORD_TO_REAL((T_PLC_US() - start) / cycles)/1000000;                                  | nan                                                      |
| nan                        | mode := 4;                                                                                      | nan                                                      |
| 4:                         | (* integer arithmetik Test *)                                                                   | nan                                                      |
| nan                        | start := tx;                                                                                    | nan                                                      |
| nan                        | cycles := 0;                                                                                    | nan                                                      |
| nan                        | REPEAT                                                                                          | nan                                                      |
| nan                        | nan                                                                                             | cycles := cycles + 1;                                    |
| nan                        | nan                                                                                             | TEST_INT();                                              |
| nan                        | UNTIL (Cycles > C_max) OR ((T_PLC_US() - start) >= t_max) END_REPEAT;                           | nan                                                      |
| nan                        | T_INT := DWORD_TO_REAL((T_PLC_US() - start) / cycles)/1000000;                                  | nan                                                      |
| nan                        | mode := 5;                                                                                      | nan                                                      |
| 5:                         | (* Floating Point Arithmetik test *)                                                            | nan                                                      |
| nan                        | start := tx;                                                                                    | nan                                                      |
| nan                        | cycles := 0;                                                                                    | nan                                                      |
| nan                        | REPEAT                                                                                          | nan                                                      |
| nan                        | nan                                                                                             | cycles := cycles + 1;                                    |
| nan                        | nan                                                                                             | TEST_FLOAT();                                            |
| nan                        | UNTIL (Cycles > C_max) OR ((T_PLC_US() - start) >= t_max) END_REPEAT;                           | nan                                                      |
| nan                        | T_FLOAT := DWORD_TO_REAL((T_PLC_US() - start) / cycles)/1000000;                                | nan                                                      |
| nan                        | mode := 6;                                                                                      | nan                                                      |
| 6:                         | (* array sorting test *)                                                                        | nan                                                      |
| nan                        | start := tx;                                                                                    | nan                                                      |
| nan                        | cycles := 0;                                                                                    | nan                                                      |
| nan                        | REPEAT                                                                                          | nan                                                      |
| nan                        | nan                                                                                             | cycles := cycles + 1;                                    |
| nan                        | nan                                                                                             | TEST_ARRAY();                                            |
| nan                        | UNTIL (Cycles > C_max) OR ((T_PLC_US() - start) >= t_max) END_REPEAT;                           | nan                                                      |
| nan                        | T_ARRAY := DWORD_TO_REAL((T_PLC_US() - start) / cycles)/1000000;                                | nan                                                      |
| nan                        | mode := 0;                                                                                      | nan                                                      |
| END_CASE;                  | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FUNCTION TEST_ARRAY : BYTE | nan                                                                                             | nan                                                      |
| VAR_INPUT                  | nan                                                                                             | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR CONSTANT               | nan                                                                                             | nan                                                      |
| nan                        | X : BYTE := 2#11110000;                                                                         | nan                                                      |
| nan                        | Y : BYTE := 2#01010101;                                                                         | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR                        | nan                                                                                             | nan                                                      |
| nan                        | ta : ARRAY[0..22] OF REAL;                                                                      | nan                                                      |
| nan                        | i: INT;                                                                                         | nan                                                      |
| nan                        | t : REAL := 3.14;                                                                               | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | _array_sort(ADR(ta), SIZEOF(ta));                                                               | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FUNCTION TEST_FLOAT : REAL | nan                                                                                             | nan                                                      |
| VAR_INPUT                  | nan                                                                                             | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR CONSTANT               | nan                                                                                             | nan                                                      |
| nan                        | X : REAL := 3.1415;                                                                             | nan                                                      |
| nan                        | Y : REAL := 200000.23454;                                                                       | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR                        | nan                                                                                             | nan                                                      |
| nan                        | i: INT;                                                                                         | nan                                                      |
| nan                        | t : REAL := 3.14;                                                                               | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FOR i := 1 TO 500 DO       | nan                                                                                             | nan                                                      |
| nan                        | TEST_FLOAT := EXP(LOG(TRUNC(LN(ABS((EXPT(y/X,X)-y+x)/Y)*COS(0.5)*SIN(0.5)*TAN(0.5)))*SQRT(X))); | nan                                                      |
| END_FOR;                   | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FUNCTION TEST_INT : INT    | nan                                                                                             | nan                                                      |
| VAR_INPUT                  | nan                                                                                             | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR CONSTANT               | nan                                                                                             | nan                                                      |
| nan                        | X : INT := 21768;                                                                               | nan                                                      |
| nan                        | Y : INT := -657;                                                                                | nan                                                      |
| nan                        | Z : INT := 3;                                                                                   | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR                        | nan                                                                                             | nan                                                      |
| nan                        | i: INT;                                                                                         | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FOR i := 1 TO 1000 DO      | nan                                                                                             | nan                                                      |
| nan                        | TEST_INT := LIMIT(Y,ABS(DINT_TO_INT(Y * Y - Y +X) MOD Z)/(x-y),X) * Y -Z;                       | nan                                                      |
| END_FOR;                   | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FUNCTION TEST_L32 : DWORD  | nan                                                                                             | nan                                                      |
| VAR_INPUT                  | nan                                                                                             | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR CONSTANT               | nan                                                                                             | nan                                                      |
| nan                        | X : DWORD := 2#11110000_11111111_00000000_11110000;                                             | nan                                                      |
| nan                        | Y : DWORD := 2#01010101_00001111_11001100_00011100;                                             | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR                        | nan                                                                                             | nan                                                      |
| nan                        | i: INT;                                                                                         | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FOR i := 1 TO 1000 DO      | nan                                                                                             | nan                                                      |
| nan                        | TEST_L32 := NOT(ROL(ROR(SHL(X XOR Y,12) AND SHR(X OR Y,13),14),13)) XOR Y AND X;                | nan                                                      |
| END_FOR;                   | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FUNCTION TEST_L8 : BYTE    | nan                                                                                             | nan                                                      |
| VAR_INPUT                  | nan                                                                                             | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR CONSTANT               | nan                                                                                             | nan                                                      |
| nan                        | X : BYTE := 2#11110000;                                                                         | nan                                                      |
| nan                        | Y : BYTE := 2#01010101;                                                                         | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| VAR                        | nan                                                                                             | nan                                                      |
| nan                        | i: INT;                                                                                         | nan                                                      |
| END_VAR                    | nan                                                                                             | nan                                                      |
| nan                        | nan                                                                                             | nan                                                      |
| FOR i := 1 TO 1000 DO      | nan                                                                                             | nan                                                      |
| nan                        | TEST_L8 := NOT(ROL(ROR(SHL(X XOR Y,4) AND SHR(X OR Y,4),4),3)) XOR Y AND X;                     | nan                                                      |
| END_FOR;                   | nan                                                                                             | nan                                                      |


# Sheet: Tabelle3

*(Empty sheet)*
