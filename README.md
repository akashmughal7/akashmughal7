import SoftwareDeveloper from 'akash'; 
import { Languages, Frameworks } from 'akash/skills';

class Bio extends SoftwareDeveloper {
  name     = 'Akash Ali';
  title    = 'Senior Software Developer';
  location = 'Lahore,Punjab,Pakistan';
}

class Skills extends SoftwareDeveloper {
  languages  = ['JavaScript', 'PHP'];
  databases  = ['MySQL', 'MongoDB'];
  frameworks = ['Vue', 'Laravel'];
}


name: Waka Readme

on:
  workflow_dispatch:
  schedule:
    # Runs at 12am UTC
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: Update this repo's README
    runs-on: ubuntu-latest
    steps:
      - uses: athul/waka-readme@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
