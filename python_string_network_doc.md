# 📘 Python String Operations & Networking Examples
This documentation covers basic to advanced string manipulation techniques in Python, with networking context and expected outputs.


## 🔹 String Basics & Memory Info

```python
box = "Apple"
print(box)
print(type(box))

# Memory address
print(id(box))
```

**✅ Output:**
```text
Apple
<class 'str'>
140448083084848
```

## 🔹 Positive & Negative Indexing

```python
box = "Sugar"
print(box[0])  # 'S'
print(box[-1]) # 'r'
```

**✅ Output:**
```text
S
r
```

## 🔹 Slicing and Step

```python
python = "This_is_NetG_India"
print(python[0:4])     # 'This'
print(python[8:12])    # 'NetG'
print(python[-5:])     # 'India'
print(python[::-1])    # 'aidnI_GteN_si_sihT'
```

**✅ Output:**
```text
This
NetG
India
aidnI_GteN_si_sihT
```

## 🔹 Using str.format() for Networking Commands

```python
ping_cmd = "ping {} source {}"
print(ping_cmd.format("2.2.2.2", "1.1.1.1"))
```

**✅ Output:**
```text
ping 2.2.2.2 source 1.1.1.1
```

## 🔹 VLAN Concatenation with str()

```python
vlan = "vlan"
vlan_id = 10
result = vlan + str(vlan_id)
print(result)
```

**✅ Output:**
```text
vlan10
```

## 🔹 IP Address Classification (using split)

```python
ip = "192.168.2.1"
parts = ip.split(".")
if parts[0] == "192" and parts[1] == "168":
    print(f"{ip} is a Private IP of Class C")
```

**✅ Output:**
```text
192.168.2.1 is a Private IP of Class C
```