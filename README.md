# 何曾梦觉 · 曲

这里放《何曾梦觉》的歌，给角色卡里的音乐播放器「曲」用。播放器每次打开会读这个仓库里的 `playlist.json`，按里面的顺序放。

jsDelivr 只肯给 50 MB 以内的仓库加速，超了会回 403。这个仓库九首、约 45 MB，不再加歌。

2026-11-08 起新歌放在 `hcmj-music-2`：现在有半镜、深宫曲、红尘心，约 14 MB，还能再放三十几 MB。歌单仍是这里这一份。

## 加一首新歌

1. **先擦标签**：Suno 导出的 mp3 里写着用户名和歌曲 id，只留歌名再传。
2. 找一个加上这首还不到 50 MB 的仓库，把 mp3 传进去。都满了就新建一个公开仓库 `hcmj-music-2`，以此类推。文件名只用小写英文、数字和短横线，比如 `new-song.mp3`。
3. 在这里的 `playlist.json` 的 `songs` 里加一行：`{ "title": "新歌名", "file": "new-song.mp3", "repo": "hcmj-music-2" }`。放在这个仓库里的歌不用写 `repo`。上一行末尾记得补逗号。
4. 不用更新角色卡。想马上出现，打开 `https://purge.jsdelivr.net/gh/willwefind/hcmj-music@main/playlist.json` 清一下缓存；不清的话大约 12 小时内出现。
