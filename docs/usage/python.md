## Requirements and Prequisites
- A running OpenTelemetry collector (see below)
- Python + Requests module

## Basic Python Usage

`python3 tracepusher.py -h` or `python3 tracepusher.py --help` shows help text.

```
python tracepusher.py \
--endpoint http(s)://OTEL-COLLECTOR-ENDPOINT:4318 \
--service-name service_name \
--span-name spanA \
--duration 2
```

### Optional Parameters

```
--dry-run True|False
--debug True|False
--time-shift True|False
--parent-span-id <16 character hex id>
--trace-id <32 character hex id>
--span-id <16 character hex id>
--span-attributes key=value [key2=value2...]
```

For information on span atttributes and span attribute types, see [Span Attribute Types](../reference/span-attribute-types.md).

For multi-span traces, see [multi span traces](../reference/multi-span-traces.md)
