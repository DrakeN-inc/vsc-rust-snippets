# The __Rust Short Snippets__ extension

## The best short snippets for Rust programming language to save your time.

#### P.s. If you have an idea to new snippets then write to me, thank's!
* Telegram: _[DrakeN_inc](https://t.me/DrakeN_inc)_
* GitHub: _[DrakeN-inc](https://github.com/DrakeN-inc/vsc-rust-snippets.git)_


## Comments:
| Prefix:           | Result:                                               |
| ----------------- | ----------------------------------------------------- |
| /d                | /// ...                                               |
| /e                | /// # Examples: ...                                   |
| /p                | /// # Examples: ...  # Dependencies: ...              |
| /!d               | //! ...                                               |
| /!e               | //! # Examples: ...                                   |
| /!p               | //! # Examples: ...  # Dependencies: ...              |
| /t                | // TODO: ...                                          |
| /f                | // FIX: ...                                           |
| /n                | // NOTE: ...                                          |
| hello             | "Hello, world!"                                       |
| lorem             | "Lorem ipsum dolor ..."                               |


## Attributes:
| Prefix:           | Result:                                               |
| ----------------- | ----------------------------------------------------- |
| #allow            | #[allow(...)]                                         |
| #derive           | #[derive(...)]                                        |
| #cfg              | #[cfg(...)]                                           |
| #test             | #[test]                                               |
| #doc              | #[doc = "..."]                                        |
| #!doc             | #![doc = "..."]                                       |
| #mac_exp          | #[macro_export]                                       |
| #mac_use          | #[macro_use]                                          |
| #proc             | #[proc_macro]                                         |
| #proc_attr        | #[proc_macro_attribute]                               |
| #proc_der         | #[proc_macro_derive(...)]                             |


## Operators:
| Prefix:           | Result:                                               |
| ----------------- | ----------------------------------------------------- |
| pubc              | pub(crate)                                            |
| mod               | mod name;                                             |
| use               | use name::...;                                        |
| usb               | use name::{ ... };                                    |
| usn               | use name::{\n ..., \n};                               |
| muse              | mod name;  use name::...;                             |
| musb              | mod name;  use name::{ ... };                         |
| cra               | use crate::...;                                       |
| sup               | use super::...;                                       |
| prel              | use crate::prelude::*;                                |
| ty                | type name = ...;                                      |
| le                | let name = ...;                                       |
| lm                | let mut name = ...;                                   |
| let               | let name: ... = ...;                                  |
| lem               | let mut name: ... = ...;                              |
| cons              | const name: ... = ...;                                |
| stat              | static name: ... = ...;                               |
| ret               | return ...;                                           |
| br                | break;                                                |
| bre               | break ...;                                            |
| cont              | continue;                                             |


## Blocks:
| Prefix:           | Result:                                               |
| ----------------- | ----------------------------------------------------- |
| mod               | mod { ... }                                           |
| asyn              | async { ... }                                         |
| asyb              | block_on( async { ... } )                             |
| unsf              | unsafe { ... }                                        |
| if                | if ... { ... }                                        |
| ife               | if ... { ... } else { ... }                           |
| if?               | if ... { ... }else{ ... }                             |
| ifl               | if let ... = ... { ... }                              |
| if Ok             | if let Ok(_) = ... { ... }                            |
| if Err            | if let Err(_) = ... { ... }                           |
| if Some           | if let Some(_) = ... { ... }                          |
| if None           | if let None = ... { ... }                             |
| mat               | match ... { ... => ..., }                             |
| mat Res           | match ... { Ok(v) =>, Err(e) => }                     |
| mat Opt           | match ... { Some(v) =>, None => }                     |
| fo                | for ... in ... { ... }                                |
| foi               | for i in 0...n { ... }                                |
| foe               | for (k, v) in ... { ... }                             |
| wh                | while ... { ... }                                     |
| whl               | while let ... = ... { ... }                           |
| wh Ok             | while let Ok(_) = ... { ... }                         |
| wh Err            | while let Err(_) = ... { ... }                        |
| wh Some           | while let Some(_) = ... { ... }                       |
| wh None           | while let None = ... { ... }                          |
| loo               | loop { ... }                                          |


## Structures:
| Prefix:           | Result:                                               |
| ----------------- | ----------------------------------------------------- |
| fn                | fn name(_) { ... }                                    |
| fn>               | fn name(_) -> ... { ... }                             |
| afn               | async fn name(_) { ... }                              |
| afn>              | async fn name(_) -> ... { ... }                       |
| fn>Res            | fn name(_) -> Result<T,E> { ... }                     |
| afn>Res           | async fn name(_) -> Result<T,E> { ... }               |
| fn>Opt            | fn name(_) -> Option<T> { ... }                       |
| afn>Opt           | async fn name(_) -> Option<T> { ... }                 |
| main              | fn main() -> io::Result<()> { ... }                   |
| amain             | async fn main() -> io::Result<()> { ... }             |
| test              | fn test() -> io::Result<()> { ... }                   |
| atest             | fn test() -> io::Result<()> { async{ ... } }          |
| fn new            | pub fn new(_) -> Self { ... }                         |
| fn get_           | pub fn get_(&self) -> ... { ... }                     |
| fn set_           | pub fn set_(&mut self, val: ...) { ... }              |
| fn builder        | pub fn builder() -> ... { ... }                       |
| fn build          | pub fn build(self) -> ... { ... }                     |
| fn take           | pub fn take(self) -> ... { ... }                      |
| tr                | trait Name { ... }                                    |
| im                | impl Name { ... }                                     |
| im Display        | impl Display for Name { ... }                         |
| im FromStr        | impl FromStr for Name { ... }                         |
| st                | struct Name { ... }                                   |
| stim              | struct Name { ... }  impl Name { ... }                |
| st Builder        | struct _Builder { ... }  impl _Builder { ... }        |
| en                | enum Name { ... }                                     |
| enim              | enum Name { ... }  impl Name { ... }                  |
| en Builder        | enum _Builder { ... }  impl _Builder { ... }          |
| en Error          | enum Error { ... }                ('thiserror' crate) |


## Macros:
| Prefix:           | Result:                                               |
| ----------------- | ----------------------------------------------------- |
| s!                | str!("...")                       ('add-macro' crate) |
| f!                | format!("{}", ...)                                    |
| r!                | regex!(r"...")                    ('add-macro' crate) |
| rf!               | regex!(&format!(r"{}", ...))      ('add-macro' crate) |
| v!                | vec![...]                                             |
| vd!               | vec_deque![...]                   ('add-macro' crate) |
| hm!               | hash_map!{ ... =>, }              ('add-macro' crate) |
| hs!               | hash_set![...]                    ('add-macro' crate) |
| bm!               | btree_map!{ ... =>, }             ('add-macro' crate) |
| bs!               | btree_set![...]                   ('add-macro' crate) |
| ll!               | linked_list![...]                 ('add-macro' crate) |
| bh!               | binary_heap![...]                 ('add-macro' crate) |
| bn!               | bson!{...}                             ('bson' crate) |
| rbn!              | rawbson!{...}                          ('bson' crate) |
| d!                | doc!{...}                              ('bson' crate) |
| rd!               | rawdoc!{...}                           ('bson' crate) |
| pr!               | print!("...")                                         |
| prf!              | print!("{}", ...)                                     |
| pln!              | println!("...")                                       |
| plf!              | println!("{}", ...)                                   |
| iln!              | inputln!("...")                   ('add-macro' crate) |
| ilf!              | inputln!("{}", ...)               ('add-macro' crate) |
| pan!              | panic!("...")                                         |
| paf!              | panic!("{}", ...)                                     |
| tod!              | todo!("...")                                          |
| tof!              | todo!("{}", ...)                                      |
| dbg!              | dbg!(...)                                             |
| ass!              | assert!(...)                                          |
| ase!              | assert_eq!(..., ...)                                  |
| mac!              | macro_rules! name { ... }                             |
| pari!             | parse_macro_input!(input as ...)                      |
| quo!              | quote! { ... }                                        |


## Methods:
| Prefix:           | Result:                                               |
| ----------------- | ----------------------------------------------------- |
| .in               | .into()                                               |
| .own              | .to_owned()                                           |
| .as_s             | .as_str()                                             |
| .as_b             | .as_bytes()                                           |
| .to_s             | .to_string()                                          |
| .to_v             | .to_vec()                                             |
| .low              | .to_lowercase()                                       |
| .upp              | .to_uppercase()                                       |
| .ex               | .expect("...")                                        |
| .un               | .unwrap()                                             |
| .unor             | .unwrap_or(...)                                       |
| .unore            | .unwrap_or_else(...)                                  |
| .map              | .map(|v| ...)                                         |
| .mae              | .map(|(k, v)| ...)                                    |
| .merr             | .map_error(|(k, v)| ...)                              |
| .ite              | .iter()                                               |
| .inte             | .into_iter()                                          |
| .nex              | .next()                                               |
| .colt             | .collect::<...>()                                     |
| .wcap             | .with_capacity(...)                                   |
| .fu8              | .from_utf8()                                          |
| .fu8l             | .from_utf8_lossy()                                    |
| .spl              | .split("...")                                         |
| .rspl             | .rsplit("...")                                        |
| .spln             | .splitn(..., "...")                                   |
| .rspln            | .rsplitn(..., "...")                                  |
| .splo             | .split_once("...")                                    |
| .rsplo            | .rsplit_once("...")                                   |
| .splt             | .split_terminator(."...")                             |
| .rsplt            | .rsplit_terminator(."...")                            |
| .splw             | .split_whitespace()                                   |
| .fin              | .find("...")                                          |
| .rfin             | .rfind("...")                                         |
| .mats             | .matches("...")                                       |
| .rmats            | .rmatches("...")                                      |
| .rep              | .replace("...", "...")                                |
| .repn             | .replacen("...", "...", ...)                          |
| .par              | .parse()                                              |
| .nth              | .chars().nth(...)                                     |
| .get              | .get(...)                                             |
| .push             | .push(...)                                            |
| .inst             | .insert(..., ...)                                     |


## Types:
| Prefix:           | Result:                                               |
| ----------------- | ----------------------------------------------------- |
| Res               | Result<T, E>                                          |
| Opt               | Option<T>                                             |
| Mut               | Mutex<T>                                              |
| Arc               | Arc<T>                                                |
| AMut              | Arc<Mutex<T>>                                         |
| AMut::new         | Arc::new(Mutex::new(...))                             |
| Into              | Into<T>                                               |
| IntoS             | Into<String>                                          |
| From              | From<T>                                               |
| ty Result         | pub type Result<T> = std::result::Result<T, Error>;   |
| ty Handler        | pub type Handler = fn();                              |
