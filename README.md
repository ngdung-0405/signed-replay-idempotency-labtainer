# signed-replay-idempotency-labtainer

Bài thực hành Labtainer: Signed HTTP Request Replay kết hợp Race Condition Idempotency

## Cài đặt và thực hành

```bash
cd "$LABTAINER_DIR/scripts/labtainer-student"
imodule https://raw.githubusercontent.com/ngdung-0405/signed-replay-idempotency-labtainer/main/signed-replay-idempotency.tar.gz
labtainer -r signed-replay-idempotency
```

## Các lệnh chính trong bài lab
- **target-web:** `./run_target.sh` (vulnerable) | `./run_target_secure.sh` (secure) | `python3 ~/show_ledger.py` | `python3 ~/show_audit.py`
- **sec-gateway:** `./run_gateway.sh` | `python3 ~/check_rule.py` | `python3 ~/check_alert.py`
- **victim:** `./run_victim.sh`
- **attacker-web:** `./run_attacker.sh` (nhập `race-001` trước vá, `secure-001` sau vá)
- **Chấm điểm:** `checkwork`
