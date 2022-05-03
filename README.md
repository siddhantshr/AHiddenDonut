## Stacked backend developer and a noob frontend developer .\_.

```python
import datetime
import requests
import subprocess
import json
from users.types import Coders as NoLifers

class Sid(NoLifers):
    def __init__(self):
        self.name = "Siddhant Sharma"
        self.coding_languages = [
            'Python',
            'Javascript',
            'HTML',
            'CSS', # really really bad
        ]
        self.frameworks = [
            "ReactJS",
            "Tailwind CSS",
            "Django",
        ]
        self.expertise = "discord.py"
        self.started_coding_at = datetime.datetime.fromtimestamp(1604601788)

        self.likes = (
            "Women",
            "Aviation",
            "Physics"
        )
        self.dislikes = (
            "Anime",
            "Weebs",
            "MATLAB"
        )

    @property
    def _github_stats(self):
        resp = requests.get("https://api.github.com/users/AHiddenDonut")
        if resp.status_code == 200:
            _json = json.dumps(resp.json(), indent=4)
            return _json

    @property
    def _website_stats(self):
        host = "siddhantshr.me"
        ping = subprocess.Popen(
            ["ping", host, "-c", "1"],
            stdout = subprocess.PIPE,
            stderr = subprocess.PIPE
        )

        out, error = ping.communicate()
        return out.decode("utf-8")

S1D = Sid()
```

### Some of my current projects

- Working on my site [https://siddhantshr.me/](https://siddhantshr.me/)
- Working on [Hyena-Hostable](https://gitub.com/Hyena-Bot/Hyena-Hostable)
- Used to work on [https://vaxinalerts.in/](https://vaxinalerts.in/)
- Used to work on [Hyena](https://gitub.com/Hyena-Bot)
- Random projects

### Connect with me

[Discord](https://discord.com/users/711444754080071714)

### Coding Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=AHiddenDonut&theme=radical)

<!--START_SECTION:waka-->

<!--END_SECTION:waka-->
