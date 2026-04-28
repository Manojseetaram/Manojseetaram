

```markdown
<div align="center">

```rust
fn main() {
    let engineer = Engineer {
        name:    "Manoj Seetaram",
        lang:    "Rust",
        target:  "#[no_std] · bare-metal · embedded · kernels",
        runtime: None,
        gc:      false,
    };

    engineer.run(); // just iron.
}
```

</div>

---

```
NAME     : Manoj Seetaram
FROM     : India
LANG     : Rust 🦀 — only.
TARGET   : bare-metal · embedded · kernel-space · systems
RUNTIME  : None
GC       : false
STDLIB   : optional
UNSAFE   : when the hardware demands it
```

---

### `$ whoami`

> I live at the boundary between software and silicon.  
> No runtime. No garbage collector. No abstraction tax.  
> Just Rust, registers, and raw memory.

---

### `$ cat philosophy.rs`

```rust
#![no_std]
#![no_main]

// No operating system. No libc. No hand-holding.
// This is where real systems begin.

#[no_mangle]
pub extern "C" fn _start() -> ! {
    // boot. own the hardware.
    // every byte is intentional.
    loop {
        write_register(0x0, iron());
    }
}
```

---

### `$ cat stack.toml`

```toml
[systems]
language         = "Rust"
embedded         = true
bare_metal       = true
no_std           = true
no_alloc         = true
kernel_dev       = true
memory_model     = "ownership"
unsafe_allowed   = true

[targets]
arm_cortex       = true
risc_v           = true
x86_64           = true
custom_targets   = true

[crates]
embedded_hal     = true
cortex_m         = true
rtic             = true
embassy          = true
defmt            = true
probe_rs         = true
```

---

### `$ git log --oneline`

```
* [WIP] bare-metal firmware — custom embedded target
* [WIP] kernel module — Rust · no_std
* custom HAL implementation — ARM Cortex-M
* boot sequence — no libc, raw _start()
* linker script — manual memory layout
```

---

### `$ ./connect`

```bash
$ open   linkedin.com/in/manojseetaram
$ mail   manojseetaram.artytech@gmail.com
```

---

<div align="center">

```
"closest to the metal.
 furthest from the runtime."

                    — written in Rust. compiled to iron.
```

<img src="https://github-readme-stats.vercel.app/api?username=manojseetaram&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=e05d2b&text_color=888&icon_color=e05d2b" />

<img src="https://github-readme-stats.vercel.app/api/top-langs?username=manojseetaram&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=e05d2b&text_color=888" />

</div>
```

