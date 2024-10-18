# 🚀 Overview
- **Automated IT Architecture** 
- This project is designed to automate the deployment of Information Flow diagrams using GitHub Actions.
- [Mermaid](https://mermaid.js.org/) language used for this project as **Diagram as a Code**

## 📋 Requirements
- Understanding of Mermaid language : [Tutorials](https://mermaid.js.org/ecosystem/tutorials.html)

# 🛠️ How to Run
## GitHub Actions CI/CD workflow for regular deployment
1. `workflow-main.yml` for main branch 
1. `workflow-feature.yml` for feature/* branches

## Windows PC (local) for indivisual development

1. *(Optional)* Install and Activate virtual environment
    ```sh
    python -m venv {venv_name}
    ./{venv_name}/Scripts/activate.bat
    ```

1. Install the required Python packages:
    ```sh
    pip install -r mermaid/requirements.txt
    ```

1. Run the main script:
    ```sh
    python mermaid/src/mermaid.py
    ```

## Sample Mermaid Diagram
```mermaid
graph LR
    classDef local-circle fill:#0166B1,stroke:#333,stroke-width:2px,color:#ffffff;
    classDef local-rectangle fill:#0166B1,stroke:#333,stroke-width:2px,color:#ffffff;
    classDef security fill:#000000,stroke:#333,stroke-width:2px,color:#ffffff;
    classDef central fill:#6F6F6F,stroke:#333,stroke-width:2px,color:#ffffff;
    classDef highlight stroke:red,stroke-width:6px,color:#ffffff;
    AA(["AA"])
    AB(["BB"])
    AC(["CC"])
    AD(["DD"])
    AE["EE"]
    AF["FF"]
    AG["GG"]
    AI["HH"]
    AJ["II"]
    AK(["JJ"])
    AL["KK"]
    AN(["LL"])
    AP["NN"]
    AQ(["OO"])
    AV["QQ"]
    AW["RR"]
    AY(["TT"])
    BA["VV"]
    BB["WW"]
    BC(("YY"))
    AY -->|Interface-1| AL
    AC -->|Interface-2| BB
    AI -->|Interface-3| AY
    AD -->|Interface-4| AY
    AD -->|Interface-5| AP
    BB -->|Interface-6| AC
    AJ -->|Interface-7| AY
    AL -->|Interface-8| AY
    AW -->|Interface-9| AB
    AA -->|Interface-10| AE
    BC -->|Interface-11| AF
    BC -->|Interface-12| AD
    BC -->|Interface-13| AQ
    AG -->|Interface-14| AY
    BA -->|Interface-15| AK
    AF -->|Interface-16| AN
    class AA local-rectangle;
    class AB local-rectangle;
    class AC local-rectangle;
    class AD local-rectangle;
    class AE central;
    class AF central;
    class AG central;
    class AI central;
    class AJ central;
    class AK local-rectangle;
    class AL central;
    class AN local-rectangle;
    class AP central;
    class AQ local-rectangle;
    class AV central;
    class AW central;
    class AY local-rectangle;
    class BA central;
    class BB central;
    class BC local-circle;
    class BE central;
    class BF central;
    class BG central;
```