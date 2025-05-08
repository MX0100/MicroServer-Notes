# 🔄 Java Object Serialization

## 🧠 What is Serialization?

**Serialization** is the process of converting a Java object into a format that can be stored or transmitted — such as:
- JSON
- Binary (byte stream)
- XML

**Deserialization** is the reverse process: restoring the object from the stored/transmitted format.

---

## ✅ Common Use Cases

| Use Case                        | Purpose                          |
|----------------------------------|----------------------------------|
| Save object to file              | e.g., local disk cache           |
| Store object in Redis            | e.g., login tokens, verification codes |
| Send object over network         | e.g., microservices, RPC         |
| Persist session across servers   | e.g., session clustering          |
| Send object through message queue| e.g., Kafka, RabbitMQ            |

---

## 💡 In Java, How?

### Mark the object as serializable:

```java
public class SmsCode implements Serializable {
  private static final long serialVersionUID = 1L;
  private String mobilePhone;
  private String code;
}
```
