# AI-driven-Personalized-Music-Composition
利用生成式AI根据用户的口味和情绪创作个性化音乐。
import random

class PersonalizedMusicComposer:
    def __init__(self):
        # Placeholder for initializing a more complex AI model for music generation.
        self.genres = ['Classical', 'Jazz', 'Pop', 'Rock', 'Electronic']
        self.emotions = ['Happy', 'Sad', 'Energetic', 'Relaxed']
        
    def get_user_preferences(self):
        """Simulate asking user for their music taste and current emotion."""
        print("Please select your favorite genre:")
        for i, genre in enumerate(self.genres, start=1):
            print(f"{i}. {genre}")
        genre_choice = int(input("Enter the number of your choice: ")) - 1
        
        print("\nHow are you feeling right now?")
        for i, emotion in enumerate(self.emotions, start=1):
            print(f"{i}. {emotion}")
        emotion_choice = int(input("Enter the number of your choice: ")) - 1
        
        return self.genres[genre_choice], self.emotions[emotion_choice]
    
    def generate_music(self, genre, emotion):
        """Generate music based on the user's genre and emotion. This is a placeholder for a more complex AI model."""
        # Simulate different musical elements based on genre and emotion
        melody = f"Melody line inspired by {genre} and {emotion}"
        rhythm = f"Rhythm pattern influenced by {genre} and {emotion}"
        
        # Combining the elements into a basic composition
        composition = f"{melody}\n{rhythm}\n"
        return composition
    
    def main(self):
        user_genre, user_emotion = self.get_user_preferences()
        print("\nGenerating your personalized music composition...\n")
        composition = self.generate_music(user_genre, user_emotion)
        print("Your personalized music composition:\n")
        print(composition)

if __name__ == "__main__":
    composer = PersonalizedMusicComposer()
    composer.main()
