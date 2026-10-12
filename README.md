# dialect-spot

Scores words for association with US, British, Australian and New Zealand English.

**Model:** [goldreal-ai/dialect-spot on Hugging Face](https://huggingface.co/goldreal-ai/dialect-spot)

## Usage

```python
import sys
from huggingface_hub import snapshot_download

path = snapshot_download("goldreal-ai/dialect-spot")
sys.path.insert(0, path)
from span_probes import load

probe = load(path)
probe.analyze("We parked the ute outside the servo")
```

## License

CC BY-SA 4.0. See the model page for details.
