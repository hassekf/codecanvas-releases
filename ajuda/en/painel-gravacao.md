---
slug: painel-gravacao
titulo: Recording the screen
resumo: Recording the CanvasCode window with app audio and microphone: format, quality, and what to do with the file afterwards.
area: paineis
nivel: basico
---

Opens with `⌘K` (type "gravação" or "gravar").

## What goes into the recording

The **CanvasCode window**, the audio the app produces, and your microphone. Nothing on top of the
window shows up in the video, and no sound from another app gets in. The output resolution comes
from the window's real size in pixels, Retina included.

macOS asks for the **Screen Recording** permission the first time, and recording does not start
without it: the panel shows the warning with the path to authorize. See
[the permissions macOS asks for](permissoes-do-mac).

## The controls

- **The center button**: starts recording, and resumes a paused recording. While recording, it is
  disabled.
- **Pause**: interrupts without ending.
- **Stop**: ends and saves the file.
- **The clock** counts the recorded time, and the line below it states the status: **Ready to
  record**, **Recording** or **Paused**.

There is no time limit.

**Pausing does not cut the stretch out.** The paused time becomes a still frame lasting as long as
the pause, in the final video.

## Window format

Four buttons that resize the **app window** before recording: **Landscape · 4K** (3840×2160),
**Landscape · 1080p** (1920×1080), **Vertical · Story** (1080×1920) and **Square** (1080×1080).

## Quality

The controls in this section only work while recording is stopped, and the panel says so when it is
under way.

- **Maximum · edit**: no bitrate target. The file is large, and it suits whoever is going to edit
  and re-encode later.
- **Balanced**: the default. The bitrate follows the window size.
- **Compact · chat**: lower bitrate, and capture at 1×, without Retina.
- **30 fps** and **60 fps**: frames per second. 60 fps produces a larger file.
- **H.264 · compatible** and **HEVC · compact**: the codec. HEVC yields a smaller file for the same
  visual result; H.264 plays in more places.
- **Audio in one track · share** and **Separate tracks · edit**: in one track, app sound and
  microphone are mixed when you stop the recording, which is what plays in any player. Separate,
  each source keeps its own track and their volumes are adjusted while editing; whoever opens the
  file without editing may hear only one.

## The recordings

Files are kept in `~/Movies/codeCanvas`, as `.mp4`, named by date and time. **Open the folder**
reveals that folder in the Finder. The list rereads the disk when the panel opens and when a
recording or a compression finishes.

Each row carries the file name, the date and the size, plus these buttons:

- **Assistir aqui no canvas**: opens the recording in a video panel.
- **Abrir no player externo**: opens it in the Mac's default player.
- **Comprimir o arquivo**: opens the compression options. It disappears while another compression is
  under way.
- **Mostrar no Finder**.
- **Apagar**.

**Double-clicking the name** enters rename mode. The extension stays; an empty or duplicate name is
refused, and the field stays open.

### Compressing

One recording at a time, with the progress on its own row, and that row's buttons disappear while it
runs.

- **How much to squeeze**: **Balanced** (a file recorded at Maximum shrinks around 5×) or **Compact**
  (half the bits of Balanced; small text loses definition).
- **Where to save**: **Save as a copy**, the default, which keeps the original and creates the
  smaller version beside it with "-comprimido" in the name; or **Overwrite the original**, which
  only swaps the file once compression completes.

## Recording without opening the panel

In **Settings → Interface**, the **Recording bar in the footer** option puts record, pause, stop and
the elapsed time in the app's footer. It starts off, and turning it off affects neither the panel nor
the voice commands.

By voice: start, pause, resume and stop the recording, and put the window in any of the four
formats.

An agent can list the existing recordings, with the date, size and path of each one. See
[the agent works the canvas](o-agente-mexe-no-canvas).
