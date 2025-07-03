;===============================================
;  🧠 GITHUB README - WRITTEN IN ASSEMBLY
;===============================================

section .identity
    db "Name: C++GPT"
    db "Role: Software Developer"
    db "Languages: C++, JavaScript, Lua, Assembly"
    db "Specialty: TF2 Cheats, Movement Simulation, UI Design"

section .status
    mov eax, [developer_mode]
    cmp eax, 1
    je .active_dev
    jmp .sleeping

.active_dev:
    db "🚀 Currently building TF2 cheat features..."
    db "🎯 Working on tickbase, prediction, and visuals."
    jmp .continue

.sleeping:
    db "💤 Taking a break... probably not."

.continue:
    db "🛠️ Open to collaboration on cool stuff."
    db "📬 Contact: [GitHub Issues / Discussions]"

section .projects
    db "🔹 GYATPREDATOR - Lua API for TF2"
    db "🔹 TF2 Cheat - Custom C++ base"
    db "🔹 JS Minecraft Client - Smooth UX"
    db "🔹 Modern UI Menu - Tailored Visual Style"

section .philosophy
    db "No bloat. No copy-paste. Just control."
    db "Minimalist, clean, fast."
    db "Your cheat is your signature."

section .skills
    xor eax, eax
    mov al, 1 ; C++
    mov ah, 1 ; Lua
    or eax, 0b00000011
    db "🧩 Bitwise brain engaged."
    db "🧪 Reverse engineering enjoyer."
    db "🧼 Clean code or no code."

section .links
    db "📎 GitHub: https://github.com/YOURUSERNAME"
    db "📎 Portfolio: Coming soon..."

section .eof
    db "Thanks for scrolling. Keep coding."
    hlt
