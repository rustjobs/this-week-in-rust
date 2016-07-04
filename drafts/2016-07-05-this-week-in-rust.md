Title: This Week in Rust 137
Number: 137
Date: 2016-07-05
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta:
safety, concurrency, and speed. This is a weekly summary of its progress and
community. Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us an
email](mailto:corey@octayn.net?subject=This%20Week%20in%20Rust%20Suggestion)!
Want to get involved? [We love
contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

This week's edition was edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [brson](https://github.com/brson).

# Updates from Rust Community

## News & Blog Posts

## New Crates & Project Updates

* [S.U.P.E.R. Android Analyzer](https://github.com/Razican/super). An Android applications vulnerability analyzer written in Rust.

# Crate of the Week

User [jkcclemens](https://users.rust-lang.org/users/jkcclemens) suggested his own [bins](https://crates.io/crates/bins) crate that lets us programmatically create pastebins and is now our Crate of the Week! Thanks, jkcclemens!

[Submit your suggestions for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [easy] [rust: List all available ABI strings in reference.md](https://github.com/rust-lang/rust/issues/34267).
* [easy] [rust: Expose the discriminant_value intrinsic](https://github.com/rust-lang/rust/issues/24263#issuecomment-228217702).
* [easy] [rustup: "target list" shows unavailable toolchains](https://github.com/rust-lang-nursery/rustup.rs/issues/299#issuecomment-228215543).
* [easy] [rustup: `rustup update` help is somewhat inaccurate](https://github.com/rust-lang-nursery/rustup.rs/issues/528#issuecomment-228216395).
* [easy] [rustup: Add `rustup man`](https://github.com/rust-lang-nursery/rustup.rs/issues/490#issuecomment-228220481).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

76 pull requests were [merged in the last two weeks][merged].

[merged]: https://github.com/issues?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2016-06-20..2016-06-27

* [`CharRange` is gone, `pthread_t` is stable](https://github.com/rust-lang/rust/pull/34399)
* [Macros are hygienic again (beta/nightly)](https://github.com/rust-lang/rust/pull/34374)
* [`thread::sleep(_)` can now sleep *really* long](https://github.com/rust-lang/rust/pull/34363) (Sleeping Beauty has nothing on us, folks :smile:)
* [`MultiItemModifier` may now return zero or more items](https://github.com/rust-lang/rust/pull/34253)
* [`thread_local!(..)` accepts multiple bindings](https://github.com/rust-lang/rust/pull/34077)
* [`assert_eq!(..)` now accepts an optional custom error message](https://github.com/rust-lang/rust/pull/33976)
* [no more `return_address` intrinsic](https://github.com/rust-lang/rust/pull/34491) (possibly breaking change, though crater is happy)
* [The playground backend is now written in Rust](https://github.com/rust-lang/rust-playpen/pull/187) (it actually was a python script before, yay for dogfooding!)

## New Contributors

* Alexander Stocko
* cgswords
* Fabian Vogt
* Joseph Dunne
* Mitsunori Komatsu
* Nathan Moos
* Nikhil Shagrithaya
* Paul Jarrett

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [RFC 1618: Remove the one-type-only restriction on `format_args!` arguments](https://github.com/rust-lang/rfcs/pull/1618).
* [RFC 1522: Add a initial, minimal form of `impl Trait`](https://github.com/rust-lang/rfcs/pull/1522).

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now. [This week's FCPs][fcp] are:

[fcp]: https://github.com/rust-lang/rfcs/labels/final-comment-period

* [Refine the unguarded-escape-hatch from RFC 1238 (nonparametric dropck)](https://github.com/rust-lang/rfcs/pull/1327).
* [Introduce more conventions around documenting Rust projects](https://github.com/rust-lang/rfcs/pull/1574).
* [RFC process for formatting style and Rustfmt defaults](https://github.com/rust-lang/rfcs/pull/1607).

## New RFCs

* [Const-dependent type system (also known as, Π-types and value-types)](https://github.com/rust-lang/rfcs/pull/1657).
* [Revisiting specialization: Complementary traits](https://github.com/rust-lang/rfcs/pull/1658).
* [Introduce a new type `MoveCell<T>` in `std::cell`](https://github.com/rust-lang/rfcs/pull/1659).
* [Introduce non-panicking borrow methods on `RefCell<T>`](https://github.com/rust-lang/rfcs/pull/1660).
* [Allow `::/` as a prefix in documentation links to indicate a module-relative link](https://github.com/rust-lang/rfcs/pull/1661).

# Upcoming Events

* 6/29. Rust Community Team Meeting at #rust-community on irc.mozilla.org.
* 6/29. [Rust Dublin - Error handling in Rust](http://www.meetup.com/Rust-Dublin/events/232035542/).
* [6/29. Rust Hack and Learn](http://www.meetup.com/opentechschool-berlin/events/231600336/).
* [6/30. Zurich, Switzerland - Introduction to Rust](http://www.meetup.com/Mozilla-Meetup-Switzerland/events/231268531/).
* 7/6. Rust Community Team Meeting at #rust-community on irc.mozilla.org.
* [7/7. Rust DC: Ownership and Borrowing](http://www.meetup.com/RustDC/events/231562147/).
* [7/11. Seattle Rust Meetup](https://www.eventbrite.com/e/mozilla-rust-seattle-meetup-tickets-12222326307?aff=erelexporg).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Email [Erick Tryzelaar][erickt] or [Brian
Anderson][brson] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[erickt]: mailto:erick.tryzelaar@gmail.com
[brson]: mailto:banderson@mozilla.com

# fn work(on: RustProject) -> Money

*No jobs listed for this week.*

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> <ketralnis\> Rust is also really phobic of heap allocations […]
> <Xion\> Yes, Rust encourages everyone to be a full stack developer :)

Thanks to [Matt Brubeck](https://users.rust-lang.org/users/mbrubeck) for the suggestion.

[Submit your quotes for next week][submit]!

[submit]: http://users.rust-lang.org/t/twir-quote-of-the-week/328