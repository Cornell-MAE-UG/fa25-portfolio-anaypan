---
layout: project
title: Thermodynamics Portfolio Cycle Analysis
description: Heat Exchanger and Pump Cycle Analysis
technologies: [Thermodynamics, 4-pipe Heat Exchanger, Thermocouple, Vivosun Aquapumps, Immersion Heater, Thermometer]
image: /assets/images/Heat Exchanger System.jpg
---

## Introduction
Heat Exchangers are devices designed to transfer thermal energy between two ore more fluids at different temperatures without intermixing. These devices are widely used in engineering applications such as power plants, HVAC systems, refrigeration cycles, automotive radiators and chemical processing plants.

In this project, a group of 4 students investigated a liquid–liquid heat exchanger using water as both the hot and cold working fluids. One of the water buckets had an immersion heater placed in it to warm up the water. Two pumps circulated water from hot and cold reservoirs through a heat exchanger configured initially in parallel. This system allowed changes to operating conditions such as flow arrangement and rate to observe how performance is affected. The heat exchanger is not actually operating adiabatically as it absorbs heat from the outside world as well as our fingers when the heat exchanger was adjusted to flow in either parallel or counterflow.

## Device Description and Setup
The system consisted of a heat exchanger with 4 tubes connected to 4 ports, with each tube going into a separate bucket. Two buckets, the hot and cold reservoirs, were placed next to each other. The hot reservoir had an immersion heater and was the cold was filled with ice. The remaining two buckets, placed across from the hot and cold reservoirs, were the reservoirs of what they were receiving. The heat exchanger consisted of two separate internal flow passages which allowed the hot and cold water to flow adjacent to each other while remaining physically separated by a solid wall. The pumps were used to circulate the fluids, and the flow arrangement was changed between parallel flow and counterflow by physically changing the placement of the tubes in the empty buckets. Temperature measurements at the reservoirs allowed for evaluation of performance of the heat transfer.

Heat was transferred from the hot fluid to the cold fluid in one of three ways: Convention from the hot water to the heat exchanger wall, Convection through the wall, and from the wall to the cold water. 

## System Diagram (Control Volume)
**Image 1**
/assets/images/Heat Exchanger System.jpg

**Image 2**
/assets/images/heat_exchanger_system_2.HEIC

**Schematic 1 - Parallel Flow (Max Flow Rate)**
                    Q̇_loss
                      ↑
        ┌─────────────────────────┐
        │        Heat Exchanger    │
        │        (Control Volume)  │
        │                           │
Hot In  │  ṁ_h , T_h,in  ─────►    │  ─────►  ṁ_h , T_h,out  Hot Out
        │                           │
Cold In │  ṁ_c , T_c,in   ─────►   │  ─────►  ṁ_c , T_c,out  Cold Out
        │                           │
        └─────────────────────────┘

**Schematic 2 - Hot Counterflow (Max Flow Rate)**
                    Q̇_loss
                      ↑
        ┌─────────────────────────┐
        │        Heat Exchanger    │
        │        (Control Volume)  │
        │                           │
Hot In  │  ṁ_h , T_h,in  ─────►    │   ─────►  ṁ_h , T_h,out Hot Out
        │                           │
Cold In │  ṁ_c , T_c,in  ◄─────    │   ◄─────  ṁ_c , T_c,out Cold Out
        │                           │
        └─────────────────────────┘


## Equations
- Assumptions: Neglecting kinetic and potential energy changes, No shaft work(Q=0), System at Steady State, Heat transfer Occurs only Between Streams
**Mass Balance**
Overall Steady State Balance:
Σm<sub>in</sub> = Σm<sub>out</sub>

Steady State Balance of Each Process:
m<sub>hot,in</sub> = m<sub>hot,out</sub>
m<sub>cold,in</sub> = m<sub>cold,out</sub>

**Energy Balance**
Overall Steady State Balance: 
Q + Σm<sub>in</sub>(h<sub>in</sub>) = Σm<sub>out</sub>(h<sub>out</sub>)

Energy Balance of Hot Process:
Q<sub>hot = m<sub>hot</sub>(cp)(T<sub>hot,in</sub> - T<sub>hot,out</sub>)

Energy Balance of Cold Process:
Q<sub>cold = m<sub>hot</sub>(cp)(T<sub>cold,in</sub> - T<sub>cold,out</sub>)

**Entropy Balance**
Overall Steady State Balance: 
0=∑m(s<sub>in</sub>)​−∑m(s<sub>out</sub>)​+∑T/Q​​ + S<sub>gen</sub>

With 
S<sub>gen</sub>
​

## Description of Change
In the experimentation done, the performance of the heat exchanger operating in parallel flow, counter flow and changes in rate were measured while maintaining constant inlet temperatures. The two main operating changes was reversing one look to flow in counterflow by physically reversing one loop so the one of the streams flowed in the opposite direction of other stream, and the rate of the hot stream maximized while the flow of the cold stream was minimized in both parallel and counterflow. 

## Measured Data
**Trial 1 - Parallel Flow, Both High Flow Rates**
Initial:
T<sub>cold</sub>: 280K
T<sub>hot</sub>: 314.2K

Time: 22.95 sec

After Process:
T<sub>hot</sub>: 294.0K
T<sub>cold</sub>: 297.3K

**Trial 2 - Hot Counterflow - Cold Parallel Flow, Both High Flow Rates**
Initial:
T<sub>cold</sub>: 283.0K
T<sub>hot</sub>: 307.0K

Time: 22.18 sec

After Process:
T<sub>cold</sub>: 295.1K
T<sub>hot</sub>: 292.4K


**Trial 3 - Parallel Flow, Cold Lowest Flow Rate - Hot Highest Flow Rate**
Initial:
T<sub>cold</sub>: 282.6
T<sub>hot</sub>: 307.1K

Time: 22.51 sec

After Process:
T<sub>cold</sub>: 292.2K
T<sub>hot</sub>: 296.2K

**Trial 4 - Hot Counterflow - Cold Parallel Flow, Cold Lowest Flow Rate - Hot Highest Flow Rate**
Initial:
T<sub> cold</sub>: 282.5K
T<sub>hot</sub>: 311K

Time: 22.95 sec

After Process:
T<sub>cold</sub>: 293.5K
T<sub>hot</sub>: 290.5K

**Conclusions**
In parallel flow, the hot stream cooled by 20.2K, in counterflow the hot streanmcooled by 14.6K. When the cold stream rate was increased to the lowest state (while hot remained constant at high) in parallel flow the hot stream cooled by 10.9K and in counterflow it cooled by 5.7K. This shows that there is a higher heat-transfer effectiveness in counterflow. The reasoning behind the counterflow having a higher heat-effectiveness could be due to the configuration where both reservoirs flow at their largest temperature differences (in parallel) approaching each other causing the temperature difference to be lower limiting the heat transfer. In contrast the counterflow model allows a larger temperature difference in the device increasing the heat transfer rate and overall thermal effectiveness. When the rate of the cold flow decreased, this reduced the duration of heat transfer between the hot and cold streams as the hot flow was traveling faster, so the fluids were in shorter contact with eachother reducing the transfer of heat/heat transfer. In counterflow this process contributed the most. 

## Reflections
The heat exchanger did not operate in a perfectly adiabatic manner. Though the dominant heat transfer occurs between the hot and cold water streams, heat was also exchanged with the surrounding environment as well as by direct contact from our fingers when adjusting the heat exchanger. Additionally true steady state conditions were not met and were difficult to achieve due to the small size of the hot and cold reservoirs. As the system operated, the reservoirs temperatures continuously changed due to the same quantities of water being reused across each trial. However quasi-steady-state conditions were maintained when temperature readings changed slowly over time and remained constant during the measurement periods. Adjustments could be made to improve the steady state behavior by increasing the volume of the reservoirs or continuously supplying fresh hot and cold water at fixed temperatures. This will reduce heat loss, and will allow the heat exchanger to operate closer to true steady state. The kinetic energy changes between the inlet and outlet of each flow stream are negligible for this experiment. Although the pumps were used to drive the flow of the inlets and outlets, the areas of the tubing and heat exchanger remained approximately the same resulting in similar flow velocities. So changes in kinetic energy was small compared to thermal energy changes and were neglected in the energy balance. 
