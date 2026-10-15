# gpu-status

Live status of the team's two 8x H200 Slurm nodes: <https://gitm-labs.github.io/gpu-status/>
(team password required).

* `main`: the page (`index.html`, served by GitHub Pages).
* `status`: one encrypted `status.json`, force-pushed by `gitm-job _push-status`
  on gitmachine-2 (see [GitM-Labs/runtime `deploy/h200/`](https://github.com/GitM-Labs/runtime/tree/h200-job-queue/deploy/h200)).
  It is AES-256-GCM sealed with the team password; the page decrypts it in the browser.
