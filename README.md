# ty-issues-1289

<https://github.com/astral-sh/ty/issues/1289>

```bash
uv venv
uv sync
```

```bash
23:59 $ uv pip list
Package           Version
----------------- --------
ty                0.0.1a21
typing-extensions 4.15.0
```

Make sure `extra-paths` in the `backend/pyproject.toml` is pointed to the correct python version, I tested both 3.12 and 3.13.

```bash
. .venv/bin/activate
cd backend
ty check test_ty.py
```
