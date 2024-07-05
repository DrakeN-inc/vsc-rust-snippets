# The __Rust Short Snippets__ extension

## The best short snippets for Rust programming language to save your time.

#### P.s. If you have an idea to new snippets then write to me, thank's!
* Telegram: _[DrakeN_inc](https://t.me/DrakeN_inc)_
* GitHub: _[DrakeN-inc](https://github.com/DrakeN-inc/vsc-rust-snippets.git)_


## Comments:
| Prefix:                   | Result:                                               |
| ------------------------- | ----------------------------------------------------- |
| /doc                      | /// # Examples: ...                                   |
| /doc dep                  | /// # Examples: ...  # Dependencies: ...              |
| /!doc                     | //! # Examples: ...                                   |
| /!doc dep                 | //! # Examples: ...  # Dependencies: ...              |
| /todo                     | // TODO: ...                                          |
| /fix                      | // FIX: ...                                           |
| /note                     | // NOTE: ...                                          |
| hello                     | "Hello, world!"                                       |
| lorem                     | "Lorem ipsum dolor ..."                               |


## Attributes:
| Prefix:                   | Result:                                               |
| ------------------------- | ----------------------------------------------------- |
| #allow                    | #[allow(...)]                                         |
| #derive                   | #[derive(...)]                                        |
| #cfg                      | #[cfg(...)]                                           |
| #test                     | #[test]                                               |
| #doc                      | #[doc = "..."]                                        |
| #!doc                     | #![doc = "..."]                                       |
| #error                    | #[error("...")]                   ('add-macro' crate) |
| #display                  | #[display("...")]                 ('add-macro' crate) |
| #macro_export             | #[macro_export]                                       |
| #macro_use                | #[macro_use]                                          |
| #proc_macro               | #[proc_macro]                                         |
| #proc_macro_attribute     | #[proc_macro_attribute]                               |
| #proc_macro_derive        | #[proc_macro_derive(...)]                             |


## Operators:
| Prefix:                   | Result:                                               |
| ------------------------- | ----------------------------------------------------- |
| pubcrate                  | pub(crate)                                            |
| mod                       | mod name;                                             |
| use                       | use name::...;                                        |
| use {                     | use name::{};                                         |
| mod use                   | mod name;  use name::...;                             |
| mod use {                 | mod name;  use name::{};                              |
| mod pub use               | mod name;  pub use name::...;                         |
| mod pub use {             | mod name;  pub use name::{};                          |
| crate                     | use crate::...;                                       |
| super                     | use super::...;                                       |
| prelude                   | use crate::prelude::*;                                |
| type                      | type name = ...;                                      |
| let                       | let name = ...;                                       |
| let mut                   | let mut name = ...;                                   |
| let >                     | let name: ... = ...;                                  |
| let mut >                 | let mut name: ... = ...;                              |
| const                     | const name: ... = ...;                                |
| static                    | static name: ... = ...;                               |
| return                    | return ...;                                           |
| break                     | break;                                                |
| break                     | break ...;                                            |
| continue                  | continue;                                             |


## Blocks:
| Prefix:                   | Result:                                               |
| ------------------------- | ----------------------------------------------------- |
| mod {                     | mod {}                                                |
| async {                   | async {}                                              |
| async { block_on }        | block_on( async {} )                                  |
| unsafe {                  | unsafe {}                                             |
| if                        | if ... {}                                             |
| if else                   | if ... {} else {}                                     |
| if else if                | if ... {} else if {} else {}                          |
| if?                       | if ... { }else{ }                                     |
| if let                    | if let ... = ... {}                                   |
| if let Ok                 | if let Ok(_) = ... {}                                 |
| if let Err                | if let Err(_) = ... {}                                |
| if let Some               | if let Some(_) = ... {}                               |
| if let None               | if let None = ... {}                                  |
| match                     | match ... { ... => ..., }                             |
| match Result              | match ... { Ok(v) =>, Err(e) => }                     |
| match Option              | match ... { Some(v) =>, None => }                     |
| for                       | for ... in ... {}                                     |
| for i                     | for i in 0...n {}                                     |
| for k, v                  | for (k, v) in ... {}                                  |
| while                     | while ... {}                                          |
| while let                 | while let ... = ... {}                                |
| while let Ok              | while let Ok(_) = ... {}                              |
| while let Err             | while let Err(_) = ... {}                             |
| while Some                | while let Some(_) = ... {}                            |
| while None                | while let None = ... {}                               |
| loop {                    | loop {}                                               |


## Structures:
| Prefix:                   | Result:                                               |
| ------------------------- | ----------------------------------------------------- |
| fn                        | fn name(_) {}                                         |
| fn >                      | fn name(_) -> ... {}                                  |
| fn > Result               | fn name(_) -> Result<T,E> {}                          |
| fn > Option               | fn name(_) -> Option<T> {}                            |
| fn main                   | fn main() -> io::Result<()> {}                        |
| async fn main             | async fn main() -> io::Result<()> {}                  |
| fn test                   | fn test() -> io::Result<()> {}                        |
| async fn test             | fn test() -> io::Result<()> { async{} }               |
| pub fn new                | pub fn new(_) -> Self {}                              |
| pub fn get_               | pub fn get_(&self) -> ... {}                          |
| pub fn set_               | pub fn set_(&mut self, val: ...) {}                   |
| pub fn builder            | pub fn builder() -> ... {}                            |
| pub fn build              | pub fn build(self) -> ... {}                          |
| pub fn take               | pub fn take(self) -> ... {}                           |
| trait                     | trait Name {}                                         |
| impl                      | impl Name {}                                          |
| impl Display              | impl Display for Name {}                              |
| impl FromStr              | impl FromStr for Name {}                              |
| struct                    | struct Name {}                                        |
| struct impl               | struct Name {}  impl Name {}                          |
| struct Builder            | struct _Builder {}  impl _Builder {}                  |
| enum                      | enum Name {}                                          |
| enum impl                 | enum Name {}  impl Name {}                            |
| enum Builder              | enum _Builder {}  impl _Builder {}                    |
| enum Error                | enum Error {}                     ('add-macro' crate) |
| Self {                    | Self {}                                               |


## Types:
| Prefix:                   | Result:                                               |
| ------------------------- | ----------------------------------------------------- |
| Result                    | Result<T, E>                                          |
| Option                    | Option<T>                                             |
| Mutex                     | Mutex<T>                                              |
| Arc                       | Arc<T>                                                |
| Arc<Mutex                 | Arc<Mutex<T>>                                         |
| Arc<Mutex::new            | Arc::new(Mutex::new(...))                             |
| Into                      | Into<T>                                               |
| Into<String               | Into<String>                                          |
| From                      | From<T>                                               |
| From<&str                 | From<&str>                                            |
| pub type Result           | pub type Result<T> = std::result::Result<T, Error>;   |
| pub type Handler          | pub type Handler = fn();                              |


## Macros:
| Prefix:                   | Result:                                               |
| ------------------------- | ----------------------------------------------------- |
| str!                      | str!("...")                       ('add-macro' crate) |
| format!                   | format!("{}", ...)                                    |
| regex!                    | regex!(r"...")                    ('add-macro' crate) |
| regex! format!            | regex!( format!(r"{}", ...) )     ('add-macro' crate) |
| vec!                      | vec![...]                                             |
| vec_deque!                | vec_deque![...]                   ('add-macro' crate) |
| hash_map!                 | hash_map!{ =>, }                  ('add-macro' crate) |
| hash_set!                 | hash_set![...]                    ('add-macro' crate) |
| btree_map!                | btree_map!{ =>, }                 ('add-macro' crate) |
| btree_set!                | btree_set![...]                   ('add-macro' crate) |
| linked_list!              | linked_list![...]                 ('add-macro' crate) |
| binary_heap!              | binary_heap![...]                 ('add-macro' crate) |
| bson!                     | bson!{...}                             ('bson' crate) |
| rawbson!                  | rawbson!{...}                          ('bson' crate) |
| doc!                      | doc!{...}                              ('bson' crate) |
| rawdoc!                   | rawdoc!{...}                           ('bson' crate) |
| print!                    | print!("...")                                         |
| print!,                   | print!("{}", ...)                                     |
| println!                  | println!("...")                                       |
| println!,                 | println!("{}", ...)                                   |
| input!                    | input!("...")                     ('add-macro' crate) |
| input!,                   | input!("{}", ...)                 ('add-macro' crate) |
| panic!                    | panic!("...")                                         |
| panic!,                   | panic!("{}", ...)                                     |
| todo!                     | todo!("...")                                          |
| todo!,                    | todo!("{}", ...)                                      |
| dbg!                      | dbg!(...)                                             |
| assert!                   | assert!(...)                                          |
| assert_eq!                | assert_eq!(..., ...)                                  |
| assert_ne!                | assert_ne!(..., ...)                                  |
| debug_assert!             | debug_assert!(...)                                    |
| debug_assert_eq!          | debug_assert_eq!(..., ...)                            |
| debug_assert_ne!          | debug_assert_ne!(..., ...)                            |
| macro_rules!              | macro_rules! name {}                                  |
| parse_macro_input!        | parse_macro_input!(input as ...)                      |
| quote!                    | quote! {}                                             |


## Methods:
| Prefix:                   | Result:                                               |
| ------------------------- | ----------------------------------------------------- |
| .into                     | .into()                                               |
| .to_owned                 | .to_owned()                                           |
| .as_str                   | .as_str()                                             |
| .as_os_str                | .as_os_str()                                          |
| .as_must_os_str           | .as_must_os_str()                                     |
| .as_bytes                 | .as_bytes()                                           |
| .as_path                  | .as_path()                                            |
| .to_str                   | .to_str()                                             |
| .to_string                | .to_string()                                          |
| .to_string_lossy          | .to_string_lossy()                                    |
| .to_vec                   | .to_vec()                                             |
| .to_path_buf              | .to_path_buf()                                        |
| .to_lowercase             | .to_lowercase()                                       |
| .to_uppercase             | .to_uppercase()                                       |
| .expect                   | .expect("...")                                        |
| .unwrap                   | .unwrap()                                             |
| .unwrap_or                | .unwrap_or(...)                                       |
| .unwrap_or_else           | .unwrap_or_else(...)                                  |
| .map                      | .map(|v| ...)                                         |
| .map k, v                 | .map(|(k, v)| ...)                                    |
| .map_error                | .map_error(|(k, v)| ...)                              |
| .iter                     | .iter()                                               |
| .into_iter                | .into_iter()                                          |
| .next                     | .next()                                               |
| .collect                  | .collect::<...>()                                     |
| .with_capacity            | .with_capacity(...)                                   |
| .from_utf8                | .from_utf8()                                          |
| .from_utf8_lossy          | .from_utf8_lossy()                                    |
| .split                    | .split("...")                                         |
| .rsplit                   | .rsplit("...")                                        |
| .splitn                   | .splitn(..., "...")                                   |
| .rsplitn                  | .rsplitn(..., "...")                                  |
| .split_once               | .split_once("...")                                    |
| .rsplit_once              | .rsplit_once("...")                                   |
| .split_terminator         | .split_terminator(."...")                             |
| .rsplit_terminator        | .rsplit_terminator(."...")                            |
| .split_whitespace         | .split_whitespace()                                   |
| .find                     | .find("...")                                          |
| .rfind                    | .rfind("...")                                         |
| .matches                  | .matches("...")                                       |
| .rmatches                 | .rmatches("...")                                      |
| .replace                  | .replace("...", "...")                                |
| .replacen                 | .replacen("...", "...", ...)                          |
| .parse                    | .parse()                                              |
| .chars().nth              | .chars().nth(...)                                     |
| .get                      | .get(...)                                             |
| .push                     | .push(...)                                            |
| .push_str                 | .push_str(...)                                        |
| .push_back                | .push_back(...)                                       |
| .push_front               | .push_front(...)                                      |
| .insert                   | .insert(...)                                          |
| .is_empty                 | .is_empty()                                           |
| .is_dir                   | .is_dir()                                             |
| .is_file                  | .is_file()                                            |
| .is_relative              | .is_relative()                                        |
| .is_absolute              | .is_absolute()                                        |
| .is_symlink               | .is_symlink()                                         |
