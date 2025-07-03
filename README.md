<h1 align="center">#mes</h1>
<p align="center"><i>TF2 was never meant to be played fair.</i></p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Pasted-red?style=for-the-badge&logo=ghost"/>
  <img src="https://img.shields.io/badge/C%2B%2B-Modern-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white"/>
  <img src="https://img.shields.io/badge/Engine-Source-darkgreen?style=for-the-badge&logo=steam"/>
  <img src="https://img.shields.io/badge/Game-TF2-orange?style=for-the-badge&logo=teamfortress"/>
</p>

---

```shell
mes.exe /inject | status: linked ✓
target: Team Fortress 2 | tickbase synced ✓
// mes - rewritten, reloaded, reawakened
class MES {
public:
    void Init() {
        Hook::Engine();
        Predict::Future();
        Visuals::Flex();
    }

    bool IsPasted() { return true; }
};
