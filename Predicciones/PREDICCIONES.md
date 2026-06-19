# 🏆 Predicción completa del Mundial 2026 — los 104 partidos

Generado con el modelo de este repositorio: regresores XGBoost (Tweedie) de goles + clasificador 1X2 XGBoost calibrado (isotónico), predicción a sede neutral con "efecto espejo", temperatura `T=0.27` en grupos y `T=0.5` en eliminatorias, y simulación de **Monte Carlo de 10.000 mundiales** para las probabilidades por selección.

> ⚠️ Predicción generada el 12-jun-2026, con los datos del repo (anteriores al torneo). La asignación de mejores terceros al cuadro usa la simplificación del notebook (ranking 1º-8º a huecos fijos), no la tabla oficial de la FIFA.

## Resumen

| | |
|---|---|
| 🥇 **Campeón predicho** | **🇫🇷 Francia** |
| 🥈 Subcampeón | 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra |
| 🥉 Tercer puesto | 🇪🇸 España |

### Probabilidades de ser campeón (Top 10, Monte Carlo)

| # | Selección | Campeón | Final | Semis | Cuartos |
|---|---|---|---|---|---|
| 1 | 🇫🇷 Francia | **18.2%** | 26.7% | 39.2% | 52.1% |
| 2 | 🇧🇪 Bélgica | **11.4%** | 19.0% | 33.8% | 53.9% |
| 3 | 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra | **10.2%** | 19.0% | 30.8% | 48.2% |
| 4 | 🇩🇪 Alemania | **9.8%** | 16.5% | 26.7% | 39.1% |
| 5 | 🇪🇸 España | **8.5%** | 14.8% | 26.1% | 39.6% |
| 6 | 🇦🇷 Argentina | **6.6%** | 13.7% | 24.8% | 39.3% |
| 7 | 🇵🇹 Portugal | **6.0%** | 12.6% | 23.2% | 40.4% |
| 8 | 🇳🇱 Países Bajos | **4.4%** | 9.5% | 18.6% | 39.1% |
| 9 | 🇭🇷 Croacia | **4.0%** | 8.3% | 17.4% | 31.7% |
| 10 | 🇧🇷 Brasil | **3.9%** | 8.3% | 16.0% | 32.2% |

## Fase de grupos — 72 partidos

Marcador = marcador exacto más probable según los goles esperados del modelo, condicionado al resultado 1X2 más probable.

### Grupo A

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-11 | 🇲🇽 México – 🇿🇦 Sudáfrica | **1-0** | 48% | 35% | 17% |
| 06-12 | 🇰🇷 Corea del Sur – 🇨🇿 República Checa | **2-1** | 39% | 32% | 29% |
| 06-18 | 🇨🇿 República Checa – 🇿🇦 Sudáfrica | **1-0** | 37% | 32% | 31% |
| 06-19 | 🇲🇽 México – 🇰🇷 Corea del Sur | **1-0** | 39% | 35% | 26% |
| 06-25 | 🇨🇿 República Checa – 🇲🇽 México | **1-2** | 26% | 30% | 44% |
| 06-25 | 🇿🇦 Sudáfrica – 🇰🇷 Corea del Sur | **0-1** | 24% | 34% | 42% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇲🇽 México ✅ | 9 | +1.38 |
| 2 | 🇰🇷 Corea del Sur ✅ | 6 | +0.40 |
| 3 | 🇨🇿 República Checa 🟡 | 3 | -0.61 |
| 4 | 🇿🇦 Sudáfrica | 0 | -1.17 |

### Grupo B

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-12 | 🇨🇦 Canadá – 🇧🇦 Bosnia-Herzegovina | **1-0** | 38% | 32% | 30% |
| 06-13 | 🇶🇦 Catar – 🇨🇭 Suiza | **0-2** | 16% | 31% | 54% |
| 06-18 | 🇨🇭 Suiza – 🇧🇦 Bosnia-Herzegovina | **2-1** | 42% | 31% | 26% |
| 06-19 | 🇨🇦 Canadá – 🇶🇦 Catar | **1-0** | 46% | 31% | 23% |
| 06-24 | 🇨🇭 Suiza – 🇨🇦 Canadá | **2-1** | 43% | 30% | 27% |
| 06-24 | 🇧🇦 Bosnia-Herzegovina – 🇶🇦 Catar | **2-1** | 36% | 34% | 30% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇨🇭 Suiza ✅ | 9 | +2.22 |
| 2 | 🇨🇦 Canadá ✅ | 6 | +0.02 |
| 3 | 🇧🇦 Bosnia-Herzegovina 🟡 | 3 | -0.66 |
| 4 | 🇶🇦 Catar | 0 | -1.58 |

### Grupo C

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-14 | 🇭🇹 Haití – 🏴󠁧󠁢󠁳󠁣󠁴󠁿 Escocia | **0-2** | 20% | 28% | 52% |
| 06-14 | 🇧🇷 Brasil – 🇲🇦 Marruecos | **2-1** | 50% | 28% | 22% |
| 06-20 | 🇧🇷 Brasil – 🇭🇹 Haití | **3-0** | 70% | 19% | 12% |
| 06-20 | 🏴󠁧󠁢󠁳󠁣󠁴󠁿 Escocia – 🇲🇦 Marruecos | **1-2** | 24% | 32% | 44% |
| 06-25 | 🏴󠁧󠁢󠁳󠁣󠁴󠁿 Escocia – 🇧🇷 Brasil | **0-2** | 15% | 30% | 55% |
| 06-25 | 🇲🇦 Marruecos – 🇭🇹 Haití | **2-0** | 62% | 24% | 14% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇧🇷 Brasil ✅ | 9 | +3.78 |
| 2 | 🇲🇦 Marruecos ✅ | 6 | +1.27 |
| 3 | 🏴󠁧󠁢󠁳󠁣󠁴󠁿 Escocia 🟡 | 3 | -0.65 |
| 4 | 🇭🇹 Haití | 0 | -4.40 |

### Grupo D

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-13 | 🇺🇸 EE. UU. – 🇵🇾 Paraguay | **1-0** | 44% | 30% | 27% |
| 06-14 | 🇦🇺 Australia – 🇹🇷 Turquía | **1-2** | 35% | 29% | 36% |
| 06-19 | 🇺🇸 EE. UU. – 🇦🇺 Australia | **1-0** | 36% | 33% | 31% |
| 06-20 | 🇹🇷 Turquía – 🇵🇾 Paraguay | **2-1** | 45% | 29% | 26% |
| 06-26 | 🇹🇷 Turquía – 🇺🇸 EE. UU. | **2-1** | 36% | 32% | 32% |
| 06-26 | 🇵🇾 Paraguay – 🇦🇺 Australia | **0-1** | 29% | 32% | 39% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇹🇷 Turquía ✅ | 9 | +1.19 |
| 2 | 🇺🇸 EE. UU. ✅ | 6 | +0.91 |
| 3 | 🇦🇺 Australia 🟡 | 3 | -0.54 |
| 4 | 🇵🇾 Paraguay | 0 | -1.56 |

### Grupo E

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-14 | 🇩🇪 Alemania – 🇨🇼 Curazao | **3-0** | 72% | 19% | 8% |
| 06-15 | 🇨🇮 Costa de Marfil – 🇪🇨 Ecuador | **1-0** | 43% | 34% | 23% |
| 06-20 | 🇩🇪 Alemania – 🇨🇮 Costa de Marfil | **2-1** | 47% | 36% | 17% |
| 06-21 | 🇪🇨 Ecuador – 🇨🇼 Curazao | **2-0** | 51% | 30% | 19% |
| 06-25 | 🇨🇼 Curazao – 🇨🇮 Costa de Marfil | **0-2** | 12% | 30% | 57% |
| 06-25 | 🇪🇨 Ecuador – 🇩🇪 Alemania | **0-2** | 11% | 33% | 55% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇩🇪 Alemania ✅ | 9 | +3.61 |
| 2 | 🇨🇮 Costa de Marfil ✅ | 6 | +0.88 |
| 3 | 🇪🇨 Ecuador 🟡 | 3 | -0.52 |
| 4 | 🇨🇼 Curazao | 0 | -3.97 |

### Grupo F

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-14 | 🇳🇱 Países Bajos – 🇯🇵 Japón | **1-0** | 38% | 34% | 28% |
| 06-15 | 🇸🇪 Suecia – 🇹🇳 Túnez | **2-1** | 36% | 31% | 33% |
| 06-20 | 🇳🇱 Países Bajos – 🇸🇪 Suecia | **2-1** | 52% | 29% | 19% |
| 06-21 | 🇹🇳 Túnez – 🇯🇵 Japón | **0-1** | 20% | 34% | 46% |
| 06-26 | 🇹🇳 Túnez – 🇳🇱 Países Bajos | **0-2** | 16% | 27% | 57% |
| 06-26 | 🇯🇵 Japón – 🇸🇪 Suecia | **2-1** | 45% | 34% | 22% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇳🇱 Países Bajos ✅ | 9 | +2.07 |
| 2 | 🇯🇵 Japón ✅ | 6 | +0.16 |
| 3 | 🇸🇪 Suecia 🟡 | 3 | -0.82 |
| 4 | 🇹🇳 Túnez | 0 | -1.41 |

### Grupo G

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-15 | 🇧🇪 Bélgica – 🇪🇬 Egipto | **2-0** | 61% | 28% | 11% |
| 06-16 | 🇮🇷 Irán – 🇳🇿 Nueva Zelanda | **2-0** | 54% | 31% | 15% |
| 06-21 | 🇧🇪 Bélgica – 🇮🇷 Irán | **2-0** | 48% | 32% | 20% |
| 06-22 | 🇳🇿 Nueva Zelanda – 🇪🇬 Egipto | **0-1** | 20% | 32% | 48% |
| 06-27 | 🇪🇬 Egipto – 🇮🇷 Irán | **0-1** | 20% | 34% | 45% |
| 06-27 | 🇳🇿 Nueva Zelanda – 🇧🇪 Bélgica | **0-3** | 14% | 23% | 63% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇧🇪 Bélgica ✅ | 9 | +4.20 |
| 2 | 🇮🇷 Irán ✅ | 6 | +0.56 |
| 3 | 🇪🇬 Egipto 🟡 | 3 | -0.92 |
| 4 | 🇳🇿 Nueva Zelanda | 0 | -3.84 |

### Grupo H

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-15 | 🇪🇸 España – 🇨🇻 Cabo Verde | **2-0** | 56% | 28% | 16% |
| 06-16 | 🇸🇦 Arabia Saudí – 🇺🇾 Uruguay | **0-2** | 9% | 24% | 68% |
| 06-21 | 🇪🇸 España – 🇸🇦 Arabia Saudí | **3-0** | 68% | 24% | 8% |
| 06-22 | 🇺🇾 Uruguay – 🇨🇻 Cabo Verde | **1-0** | 43% | 31% | 26% |
| 06-27 | 🇨🇻 Cabo Verde – 🇸🇦 Arabia Saudí | **1-0** | 43% | 30% | 28% |
| 06-27 | 🇺🇾 Uruguay – 🇪🇸 España | **1-2** | 18% | 36% | 46% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇪🇸 España ✅ | 9 | +3.81 |
| 2 | 🇺🇾 Uruguay ✅ | 6 | +1.25 |
| 3 | 🇨🇻 Cabo Verde 🟡 | 3 | -1.90 |
| 4 | 🇸🇦 Arabia Saudí | 0 | -3.16 |

### Grupo I

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-16 | 🇫🇷 Francia – 🇸🇳 Senegal | **2-0** | 50% | 33% | 18% |
| 06-17 | 🇮🇶 Irak – 🇳🇴 Noruega | **0-2** | 15% | 32% | 53% |
| 06-22 | 🇫🇷 Francia – 🇮🇶 Irak | **3-0** | 74% | 19% | 7% |
| 06-23 | 🇳🇴 Noruega – 🇸🇳 Senegal | **1-2** | 30% | 32% | 38% |
| 06-26 | 🇳🇴 Noruega – 🇫🇷 Francia | **0-2** | 16% | 30% | 54% |
| 06-26 | 🇸🇳 Senegal – 🇮🇶 Irak | **2-0** | 58% | 27% | 15% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇫🇷 Francia ✅ | 9 | +3.93 |
| 2 | 🇸🇳 Senegal ✅ | 6 | +1.17 |
| 3 | 🇳🇴 Noruega 🟡 | 3 | -0.97 |
| 4 | 🇮🇶 Irak | 0 | -4.13 |

### Grupo J

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-17 | 🇦🇷 Argentina – 🇩🇿 Argelia | **2-0** | 50% | 32% | 18% |
| 06-17 | 🇦🇹 Austria – 🇯🇴 Jordania | **2-0** | 74% | 20% | 6% |
| 06-22 | 🇦🇷 Argentina – 🇦🇹 Austria | **1-1** | 39% | 39% | 22% |
| 06-23 | 🇯🇴 Jordania – 🇩🇿 Argelia | **0-2** | 16% | 26% | 58% |
| 06-28 | 🇩🇿 Argelia – 🇦🇹 Austria | **0-1** | 28% | 32% | 40% |
| 06-28 | 🇯🇴 Jordania – 🇦🇷 Argentina | **0-3** | 7% | 14% | 80% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇦🇷 Argentina ✅ | 7 | +3.35 |
| 2 | 🇦🇹 Austria ✅ | 7 | +1.04 |
| 3 | 🇩🇿 Argelia 🟡 | 3 | +0.16 |
| 4 | 🇯🇴 Jordania | 0 | -4.55 |

### Grupo K

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-17 | 🇵🇹 Portugal – 🇨🇩 RD Congo | **2-0** | 58% | 27% | 15% |
| 06-18 | 🇺🇿 Uzbekistán – 🇨🇴 Colombia | **0-2** | 14% | 25% | 60% |
| 06-23 | 🇵🇹 Portugal – 🇺🇿 Uzbekistán | **2-0** | 58% | 29% | 13% |
| 06-24 | 🇨🇴 Colombia – 🇨🇩 RD Congo | **2-0** | 49% | 28% | 24% |
| 06-28 | 🇨🇩 RD Congo – 🇺🇿 Uzbekistán | **1-0** | 40% | 30% | 30% |
| 06-28 | 🇨🇴 Colombia – 🇵🇹 Portugal | **1-2** | 21% | 37% | 42% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🇵🇹 Portugal ✅ | 9 | +3.29 |
| 2 | 🇨🇴 Colombia ✅ | 6 | +1.15 |
| 3 | 🇨🇩 RD Congo 🟡 | 3 | -1.71 |
| 4 | 🇺🇿 Uzbekistán | 0 | -2.73 |

### Grupo L

| Fecha | Partido | Pred. | P(1) | P(X) | P(2) |
|---|---|:-:|--:|--:|--:|
| 06-17 | 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra – 🇭🇷 Croacia | **1-1** | 36% | 43% | 21% |
| 06-18 | 🇬🇭 Ghana – 🇵🇦 Panamá | **0-1** | 33% | 29% | 39% |
| 06-23 | 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra – 🇬🇭 Ghana | **3-0** | 67% | 20% | 12% |
| 06-24 | 🇵🇦 Panamá – 🇭🇷 Croacia | **0-2** | 13% | 27% | 61% |
| 06-27 | 🇭🇷 Croacia – 🇬🇭 Ghana | **2-0** | 62% | 24% | 14% |
| 06-27 | 🇵🇦 Panamá – 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra | **0-2** | 13% | 27% | 59% |

| Pos | Equipo | Pts | DG (xG) |
|---|---|--:|--:|
| 1 | 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra ✅ | 7 | +3.53 |
| 2 | 🇭🇷 Croacia ✅ | 7 | +2.25 |
| 3 | 🇵🇦 Panamá 🟡 | 3 | -2.98 |
| 4 | 🇬🇭 Ghana | 0 | -2.80 |

✅ clasificado directo · 🟡 tercero (pasan los 8 mejores)

## Eliminatorias — 32 partidos

Si el empate es el resultado más probable, el cruce se decide por penaltis a favor del equipo con mayor probabilidad de victoria.

### Dieciseisavos de final (16 cruces) · *28 jun - 3 jul*

| Cruce | Pred. | Avanza | P(1) | P(X) | P(2) |
|---|:-:|---|--:|--:|--:|
| 🇩🇪 Alemania – 🇩🇿 Argelia | **2-0** | **🇩🇪 Alemania** | 55% | 30% | 16% |
| 🇫🇷 Francia – 🇪🇨 Ecuador | **2-0** | **🇫🇷 Francia** | 60% | 29% | 11% |
| 🇰🇷 Corea del Sur – 🇨🇦 Canadá | **1-0** | **🇰🇷 Corea del Sur** | 38% | 32% | 30% |
| 🇳🇱 Países Bajos – 🇲🇦 Marruecos | **2-1** | **🇳🇱 Países Bajos** | 45% | 34% | 20% |
| 🇨🇴 Colombia – 🇭🇷 Croacia | **1-2** | **🇭🇷 Croacia** | 22% | 34% | 43% |
| 🇪🇸 España – 🇦🇹 Austria | **1-1 (pen)** | **🇪🇸 España** | 35% | 40% | 25% |
| 🇹🇷 Turquía – 🇦🇺 Australia | **2-1** | **🇹🇷 Turquía** | 36% | 29% | 35% |
| 🇧🇪 Bélgica – 🇨🇿 República Checa | **2-0** | **🇧🇪 Bélgica** | 59% | 27% | 14% |
| 🇧🇷 Brasil – 🇯🇵 Japón | **1-0** | **🇧🇷 Brasil** | 40% | 33% | 27% |
| 🇨🇮 Costa de Marfil – 🇸🇳 Senegal | **0-1** | **🇸🇳 Senegal** | 33% | 30% | 37% |
| 🇲🇽 México – 🏴󠁧󠁢󠁳󠁣󠁴󠁿 Escocia | **2-1** | **🇲🇽 México** | 50% | 32% | 18% |
| 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra – 🇧🇦 Bosnia-Herzegovina | **3-0** | **🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra** | 59% | 26% | 15% |
| 🇦🇷 Argentina – 🇺🇾 Uruguay | **1-0** | **🇦🇷 Argentina** | 43% | 34% | 23% |
| 🇺🇸 EE. UU. – 🇮🇷 Irán | **0-1** | **🇮🇷 Irán** | 23% | 35% | 42% |
| 🇨🇭 Suiza – 🇸🇪 Suecia | **2-1** | **🇨🇭 Suiza** | 40% | 32% | 29% |
| 🇵🇹 Portugal – 🇪🇬 Egipto | **2-0** | **🇵🇹 Portugal** | 57% | 28% | 14% |

### Octavos de final · *4 - 7 jul*

| Cruce | Pred. | Avanza | P(1) | P(X) | P(2) |
|---|:-:|---|--:|--:|--:|
| 🇩🇪 Alemania – 🇫🇷 Francia | **1-2** | **🇫🇷 Francia** | 27% | 37% | 37% |
| 🇰🇷 Corea del Sur – 🇳🇱 Países Bajos | **1-2** | **🇳🇱 Países Bajos** | 17% | 34% | 49% |
| 🇭🇷 Croacia – 🇪🇸 España | **1-1 (pen)** | **🇪🇸 España** | 20% | 44% | 36% |
| 🇹🇷 Turquía – 🇧🇪 Bélgica | **1-2** | **🇧🇪 Bélgica** | 19% | 27% | 54% |
| 🇧🇷 Brasil – 🇸🇳 Senegal | **2-1** | **🇧🇷 Brasil** | 39% | 30% | 31% |
| 🇲🇽 México – 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra | **1-2** | **🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra** | 19% | 34% | 47% |
| 🇦🇷 Argentina – 🇮🇷 Irán | **2-0** | **🇦🇷 Argentina** | 45% | 32% | 22% |
| 🇨🇭 Suiza – 🇵🇹 Portugal | **1-2** | **🇵🇹 Portugal** | 22% | 36% | 41% |

### Cuartos de final · *9 - 11 jul*

| Cruce | Pred. | Avanza | P(1) | P(X) | P(2) |
|---|:-:|---|--:|--:|--:|
| 🇫🇷 Francia – 🇳🇱 Países Bajos | **2-1** | **🇫🇷 Francia** | 43% | 37% | 20% |
| 🇪🇸 España – 🇧🇪 Bélgica | **1-1 (pen)** | **🇪🇸 España** | 31% | 38% | 31% |
| 🇧🇷 Brasil – 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra | **1-2** | **🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra** | 23% | 37% | 40% |
| 🇦🇷 Argentina – 🇵🇹 Portugal | **1-1 (pen)** | **🇵🇹 Portugal** | 29% | 41% | 30% |

### Semifinales · *14 - 15 jul*

| Cruce | Pred. | Avanza | P(1) | P(X) | P(2) |
|---|:-:|---|--:|--:|--:|
| 🇫🇷 Francia – 🇪🇸 España | **1-1 (pen)** | **🇫🇷 Francia** | 32% | 44% | 24% |
| 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra – 🇵🇹 Portugal | **1-1 (pen)** | **🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra** | 36% | 38% | 25% |

### Partido por el 3er puesto · *18 jul*

| Cruce | Pred. | Avanza | P(1) | P(X) | P(2) |
|---|:-:|---|--:|--:|--:|
| 🇪🇸 España – 🇵🇹 Portugal | **1-1 (pen)** | **🇪🇸 España** | 36% | 39% | 25% |

### 🏆 Gran Final — MetLife Stadium, Nueva York/Nueva Jersey · *19 jul*

| Cruce | Pred. | Avanza | P(1) | P(X) | P(2) |
|---|:-:|---|--:|--:|--:|
| 🇫🇷 Francia – 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra | **1-1 (pen)** | **🇫🇷 Francia** | 34% | 42% | 24% |

## Probabilidades por selección — 10.000 mundiales simulados

| Selección | Pasa grupos | Octavos | Cuartos | Semis | Final | 🏆 Campeón |
|---|--:|--:|--:|--:|--:|--:|
| 🇫🇷 Francia | 95.4% | 75.4% | 52.1% | 39.2% | 26.7% | **18.2%** |
| 🇧🇪 Bélgica | 94.3% | 73.6% | 53.9% | 33.8% | 19.0% | **11.4%** |
| 🏴󠁧󠁢󠁥󠁮󠁧󠁿 Inglaterra | 93.5% | 69.3% | 48.2% | 30.8% | 19.0% | **10.2%** |
| 🇩🇪 Alemania | 95.7% | 67.7% | 39.1% | 26.7% | 16.5% | **9.8%** |
| 🇪🇸 España | 95.3% | 59.1% | 39.6% | 26.1% | 14.8% | **8.5%** |
| 🇦🇷 Argentina | 95.2% | 58.7% | 39.3% | 24.8% | 13.7% | **6.6%** |
| 🇵🇹 Portugal | 93.0% | 62.7% | 40.4% | 23.2% | 12.6% | **6.0%** |
| 🇳🇱 Países Bajos | 88.7% | 58.5% | 39.1% | 18.6% | 9.5% | **4.4%** |
| 🇭🇷 Croacia | 90.4% | 58.6% | 31.7% | 17.4% | 8.3% | **4.0%** |
| 🇧🇷 Brasil | 94.7% | 56.0% | 32.2% | 16.0% | 8.3% | **3.9%** |
| 🇦🇹 Austria | 89.7% | 46.8% | 25.2% | 12.8% | 5.7% | **2.4%** |
| 🇸🇳 Senegal | 80.4% | 44.3% | 22.0% | 10.9% | 4.7% | **1.8%** |
| 🇲🇽 México | 85.5% | 53.3% | 23.8% | 9.3% | 4.0% | **1.5%** |
| 🇮🇷 Irán | 82.2% | 50.8% | 24.5% | 11.3% | 4.4% | **1.3%** |
| 🇺🇾 Uruguay | 86.9% | 38.4% | 19.8% | 9.8% | 3.9% | **1.3%** |
| 🇨🇭 Suiza | 87.1% | 48.3% | 22.2% | 9.3% | 3.7% | **1.2%** |
| 🇨🇮 Costa de Marfil | 82.5% | 40.0% | 18.3% | 8.1% | 3.3% | **1.2%** |
| 🇯🇵 Japón | 80.1% | 40.2% | 20.7% | 7.8% | 3.0% | **1.1%** |
| 🇨🇴 Colombia | 84.9% | 42.5% | 19.7% | 8.2% | 2.9% | **0.8%** |
| 🇳🇴 Noruega | 66.8% | 30.2% | 12.2% | 5.0% | 1.9% | **0.6%** |
| 🇲🇦 Marruecos | 84.8% | 36.1% | 17.0% | 5.7% | 1.9% | **0.6%** |
| 🇹🇷 Turquía | 78.4% | 37.6% | 13.7% | 5.1% | 1.5% | **0.6%** |
| 🇰🇷 Corea del Sur | 74.4% | 41.5% | 14.7% | 4.6% | 1.5% | **0.4%** |
| 🇩🇿 Argelia | 75.0% | 26.8% | 10.1% | 3.6% | 1.1% | **0.3%** |
| 🇨🇦 Canadá | 75.2% | 33.3% | 12.1% | 3.4% | 1.0% | **0.3%** |
| 🇨🇿 República Checa | 63.3% | 29.2% | 9.9% | 2.9% | 0.8% | **0.2%** |
| 🇸🇪 Suecia | 54.1% | 21.1% | 9.1% | 2.7% | 0.8% | **0.2%** |
| 🇺🇸 EE. UU. | 74.5% | 31.4% | 9.9% | 3.0% | 0.8% | **0.2%** |
| 🇨🇻 Cabo Verde | 56.7% | 17.1% | 6.0% | 1.7% | 0.5% | **0.2%** |
| 🇪🇨 Ecuador | 65.1% | 22.0% | 6.4% | 1.7% | 0.4% | **0.1%** |
| 🇦🇺 Australia | 69.6% | 28.8% | 9.0% | 2.6% | 0.8% | **0.1%** |
| 🇧🇦 Bosnia-Herzegovina | 63.2% | 22.7% | 7.7% | 1.9% | 0.4% | **0.1%** |
| 🇿🇦 Sudáfrica | 48.5% | 19.8% | 6.7% | 1.6% | 0.3% | **0.1%** |
| 🇨🇩 RD Congo | 51.2% | 16.8% | 5.5% | 1.7% | 0.3% | **0.1%** |
| 🇹🇳 Túnez | 45.4% | 16.0% | 6.1% | 1.5% | 0.4% | **0.1%** |
| 🏴󠁧󠁢󠁳󠁣󠁴󠁿 Escocia | 64.7% | 18.5% | 6.1% | 1.5% | 0.3% | **0.1%** |
| 🇵🇦 Panamá | 38.7% | 11.6% | 3.4% | 0.8% | 0.2% | **0.1%** |
| 🇪🇬 Egipto | 58.1% | 23.0% | 6.6% | 1.7% | 0.4% | **0.0%** |
| 🇵🇾 Paraguay | 50.9% | 15.6% | 3.6% | 0.8% | 0.2% | **0.0%** |
| 🇳🇿 Nueva Zelanda | 28.2% | 7.5% | 1.6% | 0.5% | 0.1% | **0.0%** |
| 🇺🇿 Uzbekistán | 34.7% | 8.8% | 2.2% | 0.5% | 0.1% | **0.0%** |
| 🇮🇶 Irak | 20.6% | 4.5% | 0.9% | 0.2% | 0.0% | **0.0%** |
| 🇨🇼 Curazao | 22.1% | 4.6% | 1.1% | 0.2% | 0.0% | **0.0%** |
| 🇶🇦 Catar | 44.7% | 12.3% | 2.8% | 0.5% | 0.1% | **0.0%** |
| 🇬🇭 Ghana | 35.8% | 9.7% | 2.3% | 0.4% | 0.0% | **0.0%** |
| 🇯🇴 Jordania | 12.7% | 2.0% | 0.3% | 0.1% | 0.0% | **0.0%** |
| 🇸🇦 Arabia Saudí | 23.9% | 3.5% | 0.7% | 0.1% | 0.0% | **0.0%** |
| 🇭🇹 Haití | 23.5% | 3.6% | 0.7% | 0.0% | 0.0% | **0.0%** |

## Validación con los partidos ya jugados

| Partido | Predicción del modelo | Resultado real |
|---|:-:|:-:|
| 🇲🇽 México – 🇿🇦 Sudáfrica | 1-0 (P1 48%) | 2-0 ✅ ganador acertado |
| 🇰🇷 Corea del Sur – 🇨🇿 República Checa | 2-1 (P1 39%) | 2-1 ✅ ganador acertado |

---
*Predicciones generadas automáticamente con `prediccion_mundial.py`. El fútbol, por suerte, no entiende de modelos.* ⚽