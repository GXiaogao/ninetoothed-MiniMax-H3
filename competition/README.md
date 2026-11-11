# MiniMax H3 private-runtime compatibility change

Base:upstream tagv0.26.0. The only package implementation change is in src/ninetoothed/generation.py:CACHE_DIR uses explicitly configured NINETOOTHED_CACHE_DIR instead of the home directory. See source-provenance.json for original and patched SHA256. No operator arithmetic or compiler optimization pass is changed in this report-scoped branch.

The generated gated-residual DSL/exporter/host adapter is published in the InfiniCore modification repository under competition/ninetoothed-gated-v3. Later independent Attention/LLVM/BF16 debugging is not part of this historical report snapshot and must not be presented as passed formal integration.

Use the pinned0.26.0 source or the fixed offline0.26.0 wheel in a private environment only, set NINETOOTHED_CACHE_DIR to a writable job-local directory, and compare the installed generation.py hash with source-provenance.json. The total submission install_ninetoothed_gfx936.py reproduces this exact relocation on an isolated wheel copy. Do not apply that original-to-patched transform twice. Upstream Apache2 license remains unchanged.
