
<p align="center">
    [nirvana](https://user-images.githubusercontent.com/61369603/112726486-c6b5c180-8f2e-11eb-970f-c6e6b1b62333.png)
    <p align="center">
       Nirvana - hacklenmiş e mail ve şifre bilgisi kontrolü.
	   Bu program darknet ağından sızıntı şifreleri tespit eder. penetration testi için düzenlenmiştir.
</p>

---

##### API: pwndb2am4tzkvold (dot) onion

Find leaked emails with your passwords.

---

#### Installation

Install dependencies (Debian/Ubuntu):
```
sudo apt install tor python3 python3-pip
```

Install with `pip3`:
```
sudo -H pip3 install git+https://github.com/Realradioactive/nirvana.git
nirvana --help
```

---

#### Building from Source

Clone this repository, and:
```
git clone https://github.com/Realradioactive/nirvana.git ; cd nirvana
sudo -H pip3 install -r requirements.txt
python3 setup.py build
sudo python3 setup.py install
```

---

#### Update

To update this tool to the latest version, run:
```
sudo -H pip3 install git+https://github.com/Realradioactive/archive-nirvana.git --upgrade
nirvana --version
```

---

#### Usage

Start by printing the available actions by running `nirvana --help`. It's also necessary to restart the **Tor** service `sudo service tor restart`. Then you can perform the following tests:

1. Search emails with the password: `123456789`
```
nirvana search '123456789' --password -o test1
```

2. Search emails with the just-name: `melisa`
```
nirvana search 'melisa' --just-name -o test2
```

3. Search emails with the domain: `hotmail.com`
```
nirvana search 'hotmail.com' --domain -o test3
```

4. Search email password: `melisa@unknown.com`
```
nirvana target 'melisa@unknown.com' -o test4
```

---

#### Disclaimer

Usage this program for attacking targets without prior consent is illegal. It's the end user's responsibility to obey allapplicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program.
This program is basically rearranged for use only during penetration testing.
---

#### Thanks
Realradioactive

decoxviii
pwndb_api by: M3l0nPan
pwndb by: davidtavarez


