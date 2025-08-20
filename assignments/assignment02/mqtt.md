# Exploring MQTT QoS Levels

Experiment with QoS 0, 1, and 2.
Observe how message delivery changes based on QoS settings.

## Publisher_qos.py output

```
python -u "/Users/teesinad/Documents/school/IOT/assignment/Iot-class-2025/Iot-class-2025-gateway/app/publisher_qos.py"
/Users/teesinad/Documents/school/IOT/assignment/Iot-class-2025/Iot-class-2025-gateway/app/publisher_qos.py:20: DeprecationWarning: Callback API version 1 is deprecated, update to latest version
  client = mqtt.Client()
[15:56:13] DEBUG | Sending CONNECT (u0, p0, wr0, wq0, wf0, c1, k60) client_id=b''
Enter message to publish: [15:56:13] DEBUG | Received CONNACK (0, 0)
2
Enter QoS level (0, 1, 2): 2
[15:56:20] DEBUG | Sending PUBLISH (d0, q2, r0, m1), 'b'test/qos/6520301001/temperature'', ... (1 bytes)
[15:56:20] PUBLISH REQUESTED | QoS=2 | Message='2' | msgid=1
Enter message to publish: [15:56:20] DEBUG | Received PUBREC (Mid: 1)
[15:56:20] DEBUG | Sending PUBREL (Mid: 1)
[15:56:20] DEBUG | Received PUBCOMP (Mid: 1)
[15:56:20] PUBLISHED | msgid=1
```

## Subscriber_qos.py Output

```
❯ python -u "/Users/teesinad/Documents/school/IOT/assignment/Iot-class-2025/Iot-class-2025-gateway/app/subscriber_qos.py"
/Users/teesinad/Documents/school/IOT/assignment/Iot-class-2025/Iot-class-2025-gateway/app/subscriber_qos.py:25: DeprecationWarning: Callback API version 1 is deprecated, update to latest version
  client = mqtt.Client()
[15:55:12] DEBUG | Sending CONNECT (u0, p0, wr0, wq0, wf0, c1, k60) client_id=b''
[15:55:12] DEBUG | Received CONNACK (0, 0)
[15:55:12] Connected with result code 0
[15:55:12] DEBUG | Sending SUBSCRIBE (d0, m1) [(b'test/qos/6520301001', 2)]
[15:55:12] DEBUG | Received SUBACK
```