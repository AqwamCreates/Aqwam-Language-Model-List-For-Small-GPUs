# Aqwam's Language Model List For Small GPUs

* Note: Speeds are approximate averages based on: 

  * RTX 4050 6GB + DDR5 RAM

  * Q4_0 K/V cache


### 👑 TIER S: The "Holy Trinity" (Top Tier)

> Perfect balance of quality, stability, and speed. These are your daily drivers.

| Model           | Quant   | Ingestion Speed (Read) | Generation Speed (Write) | Best Use Case            | Why It Wins                                                                                                                            |
|-----------------|---------|------------------------|--------------------------|--------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| Qwen 3.5 9B     | Q3_K_XL | ~110–160 t/s 🚀       | ~10–12 t/s                | The Perfect All-Rounder | New King. Reads huge prompts instantly. Writes with deep poetic nuance ("ancient sorrow"). Perfect balance of speed and soul.          |
| Qwen 3.5 4B     | Q4_K_XL | ~140–280 t/s⚡        | ~20–22 t/s                | Fast-Paced Chat         | Blazing fast at both reading and writing. Slightly less poetic than 9B, but incredibly responsive. Great for rapid banter.             |
| Ministral 3 14B | IQ2_M   | ~60–100 t/s 🐢        | ~7–8 t/s                  | Cinematic Storytelling  | Slowest writer, but deepest emotional depth. Use when you want to savor every word of a tragic story.                                  |

### ⚔️ TIER A: The Specialists

> Great for specific tasks (Vision, Massive Context, or Precision), but have trade-offs.

| Model | Quant | Ingestion Speed (Read) | Gen Speed (Write) | Best Use Case | The Trade-off |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Gemma 4 E4B | Q8_0 | ~80–120 t/s | ~11 t/s | Lore Accuracy | Maximum precision weights. Great for factual consistency, but sometimes lacks the "creative soul" of Qwen. |
| Gemma 4 E2B | Q8_0 | ~150–250 t/s | ~18–19 t/s | Infinite Memory (262k) | Only use if you strictly need >131k context. Very fast, but simpler personality. |
| MiniCPM-V 4.6 | Q4_K_M | ~300+ t/s 👁️ | ~35–45 t/s | Visual Analysis | The undisputed king of images. Reads screenshots instantly. Too small for long-term story arcs. |
| Ministral 3 8B | Q3_K_XL | ~90–130 t/s | ~8–10 t/s | Solid Backup | Good middle ground, but the Qwen 9B generally outperforms it in both poetry and speed. |


