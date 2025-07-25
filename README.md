Here’s a clean, structured **Day 2 README.md** for your FreeSWITCH learning repo:

---

```markdown
# FreeSWITCH Learning – Day 2

On Day 2, the focus is on understanding SIP profiles and creating a simple dialplan in FreeSWITCH.

---

## Objectives for Day 2

- Understand what SIP profiles are and their role in FreeSWITCH
- Explore default SIP profiles
- Create a basic dialplan to handle calls
- Verify configuration through FreeSWITCH CLI

---

## What are SIP Profiles?

SIP profiles define how FreeSWITCH communicates with SIP endpoints. They include:
- **IP and Port Bindings** (e.g., `5060` for SIP)
- **Authentication Settings**
- **Transport Protocols** (UDP/TCP/TLS)

FreeSWITCH provides two default profiles:
- **internal** – For local devices to register
- **external** – For communicating with external gateways or carriers

Profiles are located in:
```

/etc/freeswitch/sip\_profiles/

````

---

## Explore SIP Profiles

1. Navigate to the SIP profiles directory:
```bash
cd /etc/freeswitch/sip_profiles
````

2. Check the default internal profile:

```bash
nano internal.xml
```

3. Key parameters to review:

* `<param name="sip-ip" value="auto"/>`
* `<param name="rtp-ip" value="auto"/>`
* `<param name="dialplan" value="XML"/>`

---

## Creating a Simple Dialplan

Dialplans define how FreeSWITCH routes calls. Default dialplans are in:

```
/etc/freeswitch/dialplan/default/
```

### 1. Create a Test Extension

Open the default dialplan:

```bash
nano /etc/freeswitch/dialplan/default/01_test.xml
```

Add the following content:

```xml
<extension name="hello-world">
  <condition field="destination_number" expression="^1234$">
    <action application="answer"/>
    <action application="playback" data="ivr/ivr-welcome.wav"/>
    <action application="hangup"/>
  </condition>
</extension>
```

This creates an extension **1234**. When dialed, it:

* Answers the call
* Plays a welcome audio file
* Hangs up

### 2. Reload the Dialplan

```bash
fs_cli -x "reloadxml"
```

---

## Testing

1. Register a SIP client (e.g., Linphone or Zoiper) with the internal profile credentials.
2. Dial **1234**.
3. You should hear the welcome audio file.

---

## Resources

* [Dialplan Basics](https://freeswitch.com/confluence/display/FREESWITCH/Dialplan)
* [SIP Profiles](https://freeswitch.com/confluence/display/FREESWITCH/SIP+Profiles)

---

## Day 2 Summary

* Understood SIP profiles and their role
* Explored internal and external profiles
* Created and tested a simple dialplan

---

### Next Steps (Day 3)

* Explore user directory and authentication
* Configure and register multiple SIP users

```

---

✅ Save this as **`README.md`** inside your **Day 2 folder**.

---

👉 Do you want me to **prepare Day 3 README now** or **give you a full 7-day roadmap for the entire repo with folder structure and all README files**?
```
