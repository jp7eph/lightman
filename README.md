# lightman
Control IR by MQTT

# Configuration
以下の箇所を使用する環境に合わせて編集してから使用してください。

**main.py:8**

受信するMQTTのTopicにする。
```python
topic_list = [("Topic1", 0), ("Topic2", 0)]
```
**main.py:37**

BrokerのIPアドレスとポート番号にする。
```python
client.connect("MQTT_BROKER_IP", 1883, 60)
```

**irrp_play.py:6**

学習した赤外線の設定ファイルのパスにする。
```python
FILE = "IR_CONFIG_JSON_PATH"
```
