    //About me

    public class Information {
      private String name, school, location, major;
      private String[] languages, hobbies;

    public Information(String name, String school, String location,
        String major, String[] languages, String[] hobbies) {
        this.name = name;
        this.school = school;
        this.location = location;
        this.major = major;
        this.languages = languages;
        this.hobbies = hobbies;
    }

    public static void main(String[] args) {
        Information info = new Information(
            "Giovani Martins",
            "Bridgewater State University",
            "Brockton, MA",
            "Computer Science",
            new String[]{"Java", "Python", "HTML", "CSS"},
            new String[]{"Fitness", "Reading", "Cinematography", "GameDev"}
        );

         System.out.printf(
            "Name: %s\nSchool: %s\nLocation: %s\nMajor: %s\nLanguages: %s\nHobbies: %s\n",
            info.name, info.school, info.location, info.major,
            String.join(", ", info.languages),
            String.join(", ", info.hobbies));
        }
    }
