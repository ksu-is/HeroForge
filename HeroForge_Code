
from collections import Counter

# --- Race Functions ---
def human():
    return "You are a Human: adaptable, ambitious, and versatile."

def elf():
    return "You are an Elf: graceful, independent, and connected to nature."

def halfling():
    return "You are a Halfling: cheerful, generous, and community-driven."

def dwarf():
    return "You are a Dwarf: reliable, hardworking, and rooted in tradition."

def dragon():
    return "You are a Dragon: ambitious, commanding, and powerful."


# --- Class Functions ---
def wizard():
    return "You are a Wizard: intelligent, analytical, and curious."

def cleric():
    return "You are a Cleric: compassionate, faithful, and resilient."

def druid():
    return "You are a Druid: wise, patient, and in harmony with nature."

def bard():
    return "You are a Bard: charismatic, creative, and inspiring."

def paladin():
    return "You are a Paladin: principled, brave, and dependable."


# --- Mapping dictionaries ---
race_map = {
    "a": human,
    "b": elf,
    "c": halfling,
    "d": dwarf,
    "e": dragon
}

class_map = {
    "a": wizard,
    "b": cleric,
    "c": druid,
    "d": bard,
    "e": paladin
}


# --- Helper function to tally results ---
def get_result(answers, mapping):
    chosen = [mapping[a].__name__ for a in answers if a in mapping]
    counts = Counter(chosen)
    top_choice = counts.most_common(1)[0][0]
    # Find the function by name and call it
    for key, func in mapping.items():
        if func.__name__ == top_choice:
            return func()


# --- Main Quiz ---
def main_quiz():
    print("Hello adventurer! Let's determine your race for your character. Please answer the following questions:")

    # Race questions
    q_1 = input("1. Where do you feel most at home?\n"
                " a) In a lively town full of people\n"
                " b) In deep forests and natural places\n"
                " c) In warm, familiar settings with friends\n"
                " d) In steady, hardworking communities built on trust\n"
                " e) In places where ambition and leadership can shine\nYour answer: ")

    q_2 = input("2. How do you handle conflict?\n"
                " a) Seek compromise and adapt\n"
                " b) Stay quiet and wait for the right moment\n"
                " c) Defuse tension with humor or kindness\n"
                " d) Stand firm and hold your ground\n"
                " e) Assert yourself with commanding presence\nYour answer: ")

    q_3 = input("3. How do you usually spend your free time?\n"
                " a) Exploring new ideas or learning something useful\n"
                " b) Enjoying the outdoors and appreciating beauty\n"
                " c) Sharing food, laughter, and stories with friends\n"
                " d) Working on projects or honing a skill\n"
                " e) Pursuing goals that show strength and authority\nYour answer: ")

    q_4 = input("4. What quality defines you most?\n"
                " a) Ambitious and adaptable\n"
                " b) Fierce and independent\n"
                " c) Cheerful and generous\n"
                " d) Reliable and enduring\n"
                " e) Powerful and commanding\nYour answer: ")

    q_5 = input("5. What drives you forward?\n"
                " a) Curiosity about the wider world\n"
                " b) Desire for freedom and self-expression\n"
                " c) Love of simple pleasures and companionship\n"
                " d) Duty to your people or traditions\n"
                " e) Desire for control and influence\nYour answer: ")

    race_answers = [q_1, q_2, q_3, q_4, q_5]

    print("\nNow, let's determine your class based on your preferences. Please answer the following questions:")

    # Class questions
    q_6 = input("1. How do you prepare for a big challenge?\n"
                " a) Research thoroughly and plan ahead\n"
                " b) Pray or reflect for guidance\n"
                " c) Spend time outdoors to find balance\n"
                " d) Practice a performance or motivating speech\n"
                " e) Make a plan and commit to following through responsibly\nYour answer: ")

    q_7 = input("2. What role do you usually take in a group?\n"
                " a) The strategist who thinks ahead\n"
                " b) The caretaker who ensures everyone feels supported\n"
                " c) The guide who keeps harmony\n"
                " d) The storyteller who keeps morale high\n"
                " e) The dependable one who keeps everyone on track\nYour answer: ")

    q_8 = input("3. How do you handle setbacks?\n"
                " a) Look for patterns and adjust logically\n"
                " b) Offer reassurance and keep faith strong\n"
                " c) Adapt calmly and trust the process\n"
                " d) Lighten the mood or improvise creatively\n"
                " e) Stay firm and lead with conviction\nYour answer: ")

    q_9 = input("4. What kind of challenge excites you most?\n"
                " a) Solving puzzles or uncovering secrets\n"
                " b) Helping others through hardship\n"
                " c) Living in balance with nature\n"
                " d) Inspiring others through art or music\n"
                " e) Leading a team to victory\nYour answer: ")

    q_10 = input("5. What makes you feel most fulfilled?\n"
                 " a) Discovering something new\n"
                 " b) Knowing you helped someone in need\n"
                 " c) Feeling connected to the world around you\n"
                 " d) Sharing laughter and creativity with others\n"
                 " e) Standing by your values and doing what's right\nYour answer: ")

    class_answers = [q_6, q_7, q_8, q_9, q_10]

    # Results
    print("\n--- RESULTS ---")
    print("Your Race:")
    print(get_result(race_answers, race_map))

    print("\nYour Class:")
    print(get_result(class_answers, class_map))


if __name__ == "__main__":
    main_quiz()
