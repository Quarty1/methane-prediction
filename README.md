# methane-prediction
Predict methane emissions using cow behaviour
## Todo "methane-prediction/todo"  
## System Pipeline

```mermaid
flowchart LR
    CAM[720p Night Vision Camera]
    PI[Raspberry Pi 5]
    YOLO[YOLOv8n<br/>(Behavior Detection)]
    AGG[Behavior Time Aggregation]
    IPCC[IPCC Tier 2<br/>Methane Model]
    OUT[Methane Prediction<br/>(g/day per cow)]

    CAM --> PI
    PI --> YOLO
    YOLO --> AGG
    AGG --> IPCC
    IPCC --> OUT
```

