### Kenji Sato // Tokyo

Systems developer focusing on binary serialization protocols, zero-copy memory buffers, and low-latency IPC.

---

#### 📦 Open Source Tracks

* **[msgpack/msgpack-python](https://github.com/msgpack/msgpack-python)** — Buffer unsharing, timestamp extension decoding, and streaming unpacker limits.
* **[apache/arrow](https://github.com/apache/arrow)** — PyArrow memory pool fragmentation and record batch slicing.
* **[ijl/orjson](https://github.com/ijl/orjson)** — Fast datetime serialization and custom allocator alignment.

---

#### ⚡ Engineering Standards

1. **Zero-Copy Guarantees**: Parsers must slice views rather than allocate redundant byte copies.
2. **Defensive Bounds**: Binary headers must enforce strict length validation before memory reservation.
3. **Pre-Flight Invariant Validation**: Diffs and tests are pre-flight verified using [ZeroSlop™ CI](https://github.com/marketplace/actions/zeroslop-by-ribbsaeter-systems) for zero regressions.

---
*Python • C/Cython • ZeroSlop™ CI*
