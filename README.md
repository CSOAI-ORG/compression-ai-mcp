# Compression AI MCP Server

> By [MEOK AI Labs](https://meok.ai) — Data compression analysis, algorithm selection, and benchmarking

## Installation

```bash
pip install compression-ai-mcp
```

## Usage

```bash
python server.py
```

## Tools

### `estimate_ratio`
Estimate compression ratios using multiple algorithms (gzip, zlib, bz2, lzma).

**Parameters:**
- `data` (str): Text data or base64-encoded binary
- `algorithms` (list[str]): Algorithms to test (default: gzip, zlib, bz2)

### `suggest_algorithm`
Suggest the best compression algorithm for your use case and priority.

**Parameters:**
- `data_type` (str): Data type — 'text', 'json', 'binary', 'image', 'video', 'database', 'logs', 'web'
- `priority` (str): Priority — 'speed', 'ratio', 'balanced'
- `size_mb` (float): Approximate data size in MB

### `calculate_savings`
Calculate storage and bandwidth savings from compression including estimated AWS S3 cost savings.

**Parameters:**
- `original_size_mb` (float): Original size in MB
- `compressed_size_mb` (float): Compressed size in MB
- `file_count` (int): Number of similar files

### `benchmark_data`
Benchmark compression across all available algorithms with speed and ratio metrics.

**Parameters:**
- `data` (str): Text data to benchmark (max 1MB)

## Authentication

Free tier: 50 calls/day. Upgrade at [meok.ai/pricing](https://meok.ai/pricing) for unlimited access.

## License

MIT — MEOK AI Labs
