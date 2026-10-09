**Project**

Repository: https://github.com/Junjayyy/MLMPworkshop

Inference task: Monocular Depth Estimation

**Repo map**

Environment: pyproject.toml & requirements.txt

Entry point: run.py

Model: Depth-Anything-V2 (automatically downloads checkpoint weights) 

Input: assets/examples/demo01.jpg

Output: vis_depth/demo01.png

**Environment setup**
```text
git clone [https://github.com/Junjayyy/MLMPworkshop](https://github.com/Junjayyy/MLMPworkshop)
cd Depth-Anything-V2_official_fresh
uv python install 3.10
uv venv --python 3.10
source .venv/bin/activate
uv pip install -r requirements.txt
```

**Inference** 
```text
python run.py --encoder vits --img-path assets/examples/demo01.jpg --outdir vis_depth
```

**One real failure**

Category: Git Authentication & Divergent Branches

Root cause: GitHub no longer supports account password authentication for terminal Git operations, and the local repository history diverged from the remote initialization.

Minimal fix: Generated a Personal Access Token (PAT) and performed a force push to sync the repository.

**AI agent check**

Which AI coding agent did you use?: Gemini

What did it change?: Guided through resolving git divergent branch merges, updating remote URLs with PAT, and setting up the README structure.

How did you verify the change?: Verified that the depth map was successfully generated under vis_depth/demo01.png and successfully pushed to the GitHub repository.
