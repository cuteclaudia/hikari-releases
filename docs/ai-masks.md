# AI masks in Hikari (Object and Describe)

Hikari can select things in a photo for you, for example a person, the sky or a car, using **SAM 3** ("Segment Anything with Concepts"), an AI model published by Meta.

**The model is optional.** It isn't part of Hikari and isn't included in the download. Without it, Object and Describe offer to fetch it, and everything else in Hikari works as usual, including masks you've already made.

## Using them

In the Masking panel (M):

- **Object:** click the thing you want; each click refines the selection. Alt-click (⌥ on a Mac) a part to leave it out.
- **Describe:** type what to select, such as `sky`, `trees` or `the red car`, and press Return. Use commas for several things at once: `car, road`.
- **+ / −** under the selected mask add to it or take away from it. For example, Describe `sky`, then − ▸ Describe… `people`.
- **Edge** makes the border crisper (below 0) or softer (above 0).

## Getting the model

The first time you pick Object or Describe, Hikari asks whether to download the model:

- It's about **3.4 GB**, downloaded once.
- Its licence is Meta's **SAM License**, not Hikari's. Downloading the model means accepting Meta's terms.
- Nothing is downloaded until you choose **Download**. The download runs in the background, can be cancelled, and resumes if it's interrupted.
- Every file is checked when it arrives. A file that doesn't match the official model is deleted, never used.

### If the in-app download isn't available

If Hikari says it has no download location yet, put Meta's three model files in the model folder yourself:

- `model.safetensors`
- `vocab.json`
- `merges.txt`

The model folder is:

| System | Folder |
|---|---|
| Windows | `%APPDATA%\Hikari\models\sam3` |
| macOS | `~/Library/Application Support/Hikari/models/sam3` |
| Linux | `~/.config/hikari/models/sam3` |

The dialog has a button that opens this folder for you, and creates it if needed. Get the files from Meta's official SAM 3 release (on Hugging Face: `facebook/sam3`, which needs you to accept Meta's licence there). Hikari checks `model.safetensors` against the official file's size and checksum before using it.

## Privacy

The model runs **on your own computer**. Your photos aren't sent anywhere to be masked.

---

Hikari is by CuteClaudia. It is built on the open-source LightCraft project (MIT / Apache-2.0); see About ▸ Acknowledgements in the app. SAM 3 is Meta's, under Meta's SAM License.
