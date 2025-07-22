```markdown
This script is a simple Bash tool designed to generate `.m3u` playlists from audio or video files **recursively** in the current directory and its subdirectories. It scans for files with specified extensions and creates a playlist file with the name you provide.

Before searching, the script will ask for confirmation unless you pass the `-y` or `--yes` flag.

## Usage

```bash
./script_name <command> [playlist_name] [-y|--yes]
```

### Commands:

- `-a` or `--audio`: Creates a playlist containing all audio files (`.mp3`, `.flac`, `.aac`, `.ogg`) found recursively.
- `-v` or `--video`: Creates a playlist containing all video files (`.mp4`, `.mkv`, `.avi`) found recursively.
- `-y` or `--yes`: (Optional) Skips the confirmation prompt.

### Examples:

```bash
./script_name -a my_playlist
```
Prompts before scanning and creates `my_playlist.m3u` with all audio files.

```bash
./script_name -v movies -y
```
Creates `movies.m3u` with all video files, skipping the confirmation prompt.
```
