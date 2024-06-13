```rust
#[derive(Debug)]
struct Resume {
  name: &'static str,
  current_roles: Vec<&'static str>,
  former_roles: Vec<&'static str>,
  education: Vec<&'static str>,
  location: &'static str,
  webpage: &'static str,
  email: &'static str,
  twitter: &'static str,
  linkedin: &'static str,
}

fn main() {
  let resume = Resume {
      name: "Miquel A. Cabot",
      current_roles: vec![
          "Blockchain engineer. Senior Solidity/Rust/Web3 developer at Keyko/Masa Finance",
          "Lecturer at University of the Balearic Islands",
      ],
      former_roles: vec![
          "Senior Blockchain Developer at Ocean Protocol",
          "Senior Solidity/Web3 developer at Unizen",
      ],
      education: vec![
          "Ph.D. in Information and Communications Technology from the University of the Balearic Islands. Thesis title: Blockchain-based e-commerce protocols",
          "Master's Degree in Information Technologies from the University of the Balearic Islands",
          "Bachelor's Degree in Computer Engineering from the Open University of Catalonia",
      ],
      location: "Mallorca 🏝",
      webpage: "https://cabot.dev",
      email: "miquel@cabot.dev",
      twitter: "https://twitter.com/miquelcabot",
      linkedin: "https://www.linkedin.com/in/miquel-cabot/"
  };

  println!("{:#?}", resume);
}

```
