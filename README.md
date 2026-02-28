# CodeWars-Twice-linear--4-kyu---Passed
Consider a sequence u where u is defined as follows:

The number u(0) = 1 is the first one in u.
For each x in u, then y = 2 * x + 1 and z = 3 * x + 1 must be in u too.
There are no other numbers in u.
Ex: u = [1, 3, 4, 7, 9, 10, 13, 15, 19, 21, 22, 27, ...]

1 gives 3 and 4, then 3 gives 7 and 10, 4 gives 9 and 13, then 7 gives 15 and 22 and so on...

Task:
Given parameter n the function dbl_linear (or dblLinear...) returns the element u(n) of the ordered (with <) sequence u (so, there are no duplicates).

Example:
dbl_linear(10) should return 22

TEST CASES:
#[cfg(test)]
mod tests {
    use super::dbl_linear;

    fn testing(n: u32, exp: u32) -> () {
        println!("{} {}", dbl_linear(n), exp);
        assert_eq!(dbl_linear(n), exp)
    }
    
    #[test]
    fn basics_dbl_linear() {
        testing(10, 22);
        testing(20, 57);
        testing(30, 91);
        testing(50, 175);
        testing(100, 447);
        testing(500, 3355);
        testing(1000, 8488);
        testing(2000, 19773);
        testing(6000, 80914);
        testing(60000, 1511311);
    
        testing(9789, 153597);
        testing(14447, 245944);
        testing(12017, 203278);
        testing(5637, 75711);
        testing(10529, 165370);
        testing(12358, 210502);
        testing(12588, 214171);
        testing(10621, 166729);
        testing(14492, 247006);
        testing(14545, 247867);
        testing(2938, 33927);
        testing(10282, 161827);
        testing(10409, 163845);
        testing(4126, 51367);
        testing(14586, 248374);
        testing(11215, 180838);
        testing(7130, 103414);
        testing(14621, 249855);
        testing(10780, 168439);
        testing(8019, 117307);
        testing(14799, 253882);
        testing(3214, 37129);
        testing(5159, 68962);
        testing(12652, 214843);
        testing(5940, 80203);
        testing(1047, 8913);
        testing(11509, 188326);
        testing(4213, 52735);
        testing(3664, 42999);
        testing(1830, 18076);
        testing(12806, 216837);
        testing(6824, 99019);
        testing(12661, 214897);
        testing(12578, 214099);
        testing(13746, 234237);
        testing(7913, 113967);
        testing(11284, 181767);
        testing(12367, 210619);
        testing(6742, 96463);
        testing(6226, 83836);
        testing(7947, 115210);
        testing(14432, 245763);
        testing(1000, 8488);
        testing(14631, 250795);
        testing(8057, 117982);
        testing(2079, 20584);
        testing(5687, 76161);
        testing(7813, 112975);
        testing(5316, 71635);
        testing(11415, 184215);
    
        testing(24908, 494055);
        testing(23136, 455170);
        testing(29888, 636688);
        testing(23475, 462280);
        testing(20181, 384753);
        testing(21015, 412387);
        testing(20164, 384574);
        testing(23054, 454111);
        testing(22638, 447739);
        testing(23236, 456883);
        testing(23139, 455179);
        testing(26825, 552370);
        testing(27051, 564453);
        testing(22057, 434542);
        testing(23492, 463675);
        testing(24647, 487219);
        testing(25242, 501814);
        testing(24263, 481636);
        testing(28820, 614563);
        testing(28147, 598623);
    
        testing(31727, 673437);
        testing(34637, 754941);
        testing(38416, 887517);
        testing(37374, 858427);
        testing(31535, 671566);
        testing(39051, 897970);
        testing(32352, 686800);
        testing(37407, 858711);
        testing(32923, 708619);
        testing(38982, 896697);
        testing(31427, 670315);
        testing(39202, 900202);
        testing(31963, 678477);
        testing(33853, 729982);
        testing(38867, 895671);
        testing(34142, 737227);
        testing(39176, 899343);
        testing(38682, 891406);
        testing(34363, 743662);
        testing(38827, 895024);
    }
}
