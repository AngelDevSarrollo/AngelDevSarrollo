## Hi there 👋

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

import java.util.ArrayList;
import java.util.List;

class Dev {
    String name;
    String role;
    String ide;
    List<String> languages;
    String more;

    public Dev(String name, String role, String ide, List<String> languages, String more) {
        this.name = name;
        this.role = role;
        this.ide = ide;
        this.languages = languages;
        this.more = more;
    }

    public void printGitHubProfile() {
        System.out.println("### Ángel Giraldo's GitHub Profile ###");
        System.out.println("- Name: " + name);
        System.out.println("- Role: " + role);
        System.out.println("- IDEs: " + ide);
        System.out.println("- Languages:");
        for (String language : languages) {
            System.out.println("  - " + language);
        }
        System.out.println("- More info: " + more);
    }

    public static void main(String[] args) {
        List<String> languages = new ArrayList<>();
        languages.add("Java");
        languages.add("Kotlin");

        Dev desarrollo = new Dev(
                "Ángel Giraldo",
                "Junior Software Developer",
                "NetBeans, IntelliJ IDEA, Android Studio",
                languages,
                "https://www.linkedin.com/in/%C3%A1ngel-giraldo-programador/"
        );

        desarrollo.printGitHubProfile();
    }
}
