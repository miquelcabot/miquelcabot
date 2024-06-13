#[derive(Debug)]
struct Resume {
    name: &'static str,
    current_roles: Vec<&'static str>,
    education: Vec<&'static str>,
    location: &'static str,
    webpage: &'static str,
}

fn main() {
    let resume = Resume {
        name: "Miquel A. Cabot",
        current_roles: vec![
            "Blockchain engineer. Senior Solidity/Rust/Web3 developer at Keyko/Masa Finance",
            "Lecturer at University of the Balearic Islands",
        ],
        education: vec![
            "Ph.D. candidate from the University of the Balearic Islands",
            "Bachelor's Degree in Computer Engineering from the Open University of Catalonia",
        ],
        location: "Mallorca 🏝",
        webpage: "https://cabot.dev",
    };
    println!("{:#?}", resume);
}
