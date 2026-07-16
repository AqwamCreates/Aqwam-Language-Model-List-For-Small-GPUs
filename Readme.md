# Aqwam's Language Model List For Small GPUs

* Note: Speeds are approximate averages based on: 

  * RTX 4050 6GB VRAM + DDR5 16 GB RAM

  * Q4_0 KV cache (No noticeable quality loss)

* Average adult human has a reading speed of 3.67 - 5.83 words per second. A word consists of 1-3 tokens. Hence, the token generation speed must be at least 9 tokens per second for comfortable reading.

## Best Model Configuration List

| Model               | Quant   | Context Size | Ingestion Speed (Read) | Generation Speed (Write) | Best Use Case           | Model Details                                                                                   | Vision Capabilities Details                                                                         |
|---------------------|---------|--------------|------------------------|--------------------------|-------------------------|-------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| Bonsai Qwen 3.5 27B | Q1_0    | 65536        | ~400–600 t/s           | ~14-17                   | God Mode                | Slightly Repetitive And Has Slight Formatting Issues.                                           | Has vision, but tight.                                                                              |
| Qwen 3.5 9B         | Q3_K_XL | 131072       | ~100–170 t/s           | ~10–12 t/s               | The Perfect All-Rounder | High Time-To-First-Token. Strangely Good Quality Despite At Low Precision.                      | Has vision, but does not work with oogabooga's text generation web UI.                              |
| Qwen 3.5 9B         | Q3_K_S  | 65536        | ~700–900 t/s           | ~19–20 t/s               | Big Model, Perfect Fit  | High Time-To-First-Token. Strangely Good Quality Despite At Low Precision.                      | Has vision, but does not work with oogabooga's text generation web UI.                              |
| Qwen 3.5 4B         | Q5_K_XL | 131072       | ~60–2000 t/s           | ~20–22 t/s               | Fast-Paced Chat         | Extremely High Time-To-First-Token.                                                             | Has vision, but does not work with oogabooga's text generation web UI.                              |
| Gemma 4 E4B         | Q8_0    | 131072       | ~200–350 t/s           | ~11 t/s                  | Lore Accuracy           | High Time-To-First-Token and high precision.                                                    | Fast image ingestion speed. Low token usage. Extracts all information perfectly even if zoomed out. |
| Gemma 4 E2B         | Q8_0    | 262144       | ~400–1160 t/s          | ~18–19 t/s               | Huge Memory             | Extremely High Time-To-First-Token.                                                             | Fast image ingestion speed. Low token usage. Slightly weaker than E4B due to slight hallucinations. |
| Ministral 3 14B     | IQ2_M   | 131072       | ~2–160 t/s             | ~7–8 t/s                 | Cinematic Storytelling  | Deepest emotional depth.                                                                        | Not applicable.                                                                                     |
| MiniCPM-V 4.6       | F16     | 131072       | ~100-700 t/s           | ~35–45 t/s               | Visual Analysis         | The undisputed king of images. Reads screenshots instantly. Too small for long-term story arcs. | Not applicable.                                                                                     |

## Considerable Model Configuration List

| Model           | Quant   | Context Size | Ingestion Speed (Read) | Generation Speed (Write) | Model Details                                                                                                                                        | Vision Capabilities Details                                            |
|-----------------|---------|--------------|------------------------|--------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|
| Qwen 3.5 4B     | Q6_K_XL | 131072       | ~34–150 t/s            | ~10–12 t/s               | Not worth the trade-off of having higher quant when it can be replaced with higher parameter count for higher quality. Qwen 3.5 9B outperforms this. | Has vision, but does not work with oogabooga's text generation web UI. |
| Ministral 3 8B  | Q3_K_XL | 131072       | ~2–250 t/s             | ~8–10 t/s                | Good middle ground, but the Qwen 3.5 9B generally outperforms it in both poetry and speed.                                                           | Not applicable.                                                        |
