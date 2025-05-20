# NeuroVerse-Brain-Responsive-Meditation-Game
NeuroVerse: Brain-Responsive Meditation Game



# NeuroVerse: Brain-Responsive Meditation Game

An immersive EEG-integrated meditation game that helps users regulate their emotional state using real-time brain signals.

## Features
- Real-time brainwave tracking via Muse SDK
- Adaptive environment based on alpha/beta brain activity
- Designed for mental well-being, ADHD, and anxiety relief

## Tech Stack
Unity, C#, Muse SDK, Python, Oculus VR (optional)

## How It Works
- Alpha and beta brainwave levels are streamed into Unity
- The in-game environment adapts in response to calm/focus metrics

## Sample Code Snippets

```csharp
// EEGManager.cs
public class EEGManager : MonoBehaviour {
    public float alphaLevel, betaLevel;

    void Update() {
        alphaLevel = MuseManager.GetAlpha();
        betaLevel = MuseManager.GetBeta();
    }
}
