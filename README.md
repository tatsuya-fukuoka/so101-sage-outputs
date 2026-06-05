# SO101 SAGE Outputs

以下のリンクの実環境とシミュレーションのギャップを分析するためのSAGEを試した。

https://docs.nvidia.com/learning/physical-ai/sim-to-real-so-101/latest/15-strategy4-sage.html

こちらのドキュメントに従い実施

https://github.com/isaac-sim2real/sage/blob/main/docs/LEROBOT_REAL.md


以下のコマンドで実環境のSO101のアームでデータ収集を実施

```bash
python3 scripts/run_real.py \
    --robot-name=so101 \
    --motion-files=custom/custom_motion.txt \
    --output-folder=output \
    --robot-port=/dev/ttyACM1 \
    --robot-type=so_follower \
    --robot-id=follower_arm
```

以下の場所に保存されたデータをこのリポジトリに保存する。
```
Data saved to: /home/jetson/sage/output/real/so101/custom/custom_motion
  - /home/jetson/sage/output/real/so101/custom/custom_motion/joint_list.txt
  - /home/jetson/sage/output/real/so101/custom/custom_motion/control.csv
  - /home/jetson/sage/output/real/so101/custom/custom_motion/event.csv
  - /home/jetson/sage/output/real/so101/custom/custom_motion/state_motor.csv
[SO-101 Collector] Collection complete!
```
