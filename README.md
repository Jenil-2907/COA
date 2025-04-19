## 🚀 AssemblyX - Learn & Run Assembly Code Online

**AssemblyX** is a lightweight online platform to **write**, **run**, and **test** assembly programs in **x86**, **MIPS32**, and **ARM** architectures. Built for simplicity and learning, it lets users write assembly code and instantly view the output — all from the browser.

---

## 🔗 Useful Links

- 🌐 **AssemblyX Web App**  
  https://coa-hr8m.onrender.com  
- ⚙️ **Custom Flask API Server**  
  https://cloud-backend-gp5j.onrender.com

> 📌 You can reuse this server in your own projects too!  
> There's no public compiler API that supports all three: `x86`, `MIPS32`, and `ARM`.  
> So if *you* find one, please share it with me too :)

---

## ⚙️ Tech Stack

- **Flask** – for routing and rendering pages
- **Custom Flask API (Cloud_Backend)** – to compile and run user-submitted assembly code

---

## ⚠️ Important Note

`cloud_backend.py` is the core API that compiles and executes code for:
 `x86`,
 `mips32`,
 `ARM`

⚠️ **Must run on a Linux-based environment**, as it uses platform-specific compilers and commands.

📦 `requirements.txt` and a `Dockerfile` are included to help with setup and deployment.

---

## 📚 Learning + Practice

- Supports the learing of `x86`,`ARM`,`mips32` by providing some brief, questions that can be answered prefered language
- View solutions if stuck
- Explore curated external learning resources

> ⚠️ Assembly is tricky — no helpful error logs, just silent crashes. Knowing the assembler/emulator used is crucial.

---

## 🛠️ Architecture & Toolchain

| Architecture | Assembler & Emulator                   | Notes                              |
|--------------|----------------------------------------|------------------------------------|
| `x86`        | `nasm` + `ld` + native Linux execution | 32-bit ELF binaries (Linux only)   |
| `mips32`     | `spim`                                 | MIPS syscall-based programs        |
| `arm`        | `arm-linux-gnueabi-as/ld` + `qemu-arm` | Uses Linux syscalls like `svc #0`  |

---

## Additional features
Features that I failed to add because of time constraints and that anyone reading this can add are:
1) Small animations of data movement in the registers and operations taking place for each line of the solutions that is provided, if you complised this then you can go a bit advance and try create dynamic 
   animations for whatever code user writes.
2) Some random fact bar where you can get a random fact about assembly everytime you click on it and also the link if available for that fact's topic
3) In this web app I have done a bit of hard coding on questions and the solutions in flask script that is fine for small scale but if we want more question then it is not prefered and we can add some seperate 
   admin login where they can add questions and their solutons (Also the login is of no use for the build that I have built cause no data storing of particular user is taking place).

"Anyways, these are some additions that I wished I could have added, but due to time constraints, I failed. Else, you have the internet and your imagination — you can add this or anything else as add-ons for this web app."
