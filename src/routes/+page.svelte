<script lang="ts">
    import ceo from "../assets/ceo.jpg";
    import duggup from "../assets/duggup.png";
    import Icon from "../assets/Icon.png";
    import linkIco from "../assets/linkIco.png";
    import stevejobs from "../assets/stevejobs.jpg";
    import samaltman from "../assets/samaltman.jpg";
    import startuplesson from "../assets/startuplesson.jpg";
    import cleanshot from "../assets/cleanshot.png";
    import chevron from "../assets/chevron.png";
    import home from "../assets/home.png";
    import story from "../assets/story.png";
    import learn from "../assets/learn.png";
    import post from "../assets/post.png";
    import betterup from "../assets/betterup.jpg";
    import { Button } from "bits-ui";
    import { Separator } from "bits-ui";
    let isFollowed = false;

    function toggleFollow() {
        isFollowed = !isFollowed;
    }
</script>

<div class="">
    <div
        class="navbar flex justify-between h-16 align-middle items-center w-4/5 mx-auto mb-10"
    >
        <div
            class="flex align-center justify-center items-center"
        >
            <img class="duggup-logo" alt="The project logo" src={duggup} />
            <div class="font-bold text-xl ml-2">duggup</div>
        </div>
        <div class="flex">
            <div class="flex mx-4">
                <div class="p-1">
                    <img class="nav-icons" alt="The project logo" src={home} />
                </div>
                <div class="text-sm font-normal nav-icon-text p-1">Home</div>
            </div>
            <div class="flex mx-4">
                <div class="p-1">
                    <img class="nav-icons" alt="The project logo" src={story} />
                </div>
                <div class="text-sm font-normal nav-icon-text p-1">Explore</div>
            </div>
            <div class="flex mx-4">
                <div class="p-1">
                    <img class="nav-icons" alt="The project logo" src={learn} />
                </div>
                <div class="text-sm font-normal nav-icon-text p-1">Learn</div>
            </div>
            <div class="mx-4">
                <Button.Root class="rounded">
                    <div class="flex justify-center">
                        <img
                            class="nav-icons"
                            alt="The project logo"
                            src={post}
                        />
                        <div class="px-1">Post</div>
                    </div>
                </Button.Root>
            </div>
            <div class="flex items-center mx-4">
                <img class="nav-ceo" alt="The project logo" src={ceo} />
                <div class="text-xl font-medium px-2">Krishna Kiran</div>
                <img class="nav-chevron" alt="The project logo" src={chevron} />
            </div>
        </div>
    </div>

    <div class="flex items-center justify-center align-middle w-fit">
        <div class="intro-top flex flex-col items-center text-center mr-5">
            <img alt="The project logo" src={ceo} />
            <div class="text-2xl font-bold">Krishna<br /> Kiran</div>
        </div>
        <div class="text-sm flex flex-col w-1/2 mx-5">
            <div class="text-sm flex justify-between w-full">
                <div class="w-2/3">
                    Co-Founder and CEO at Duggup - Social network for people in
                    tech. Ex-Amazon Head of Engineering. I write hot-takes on
                    building a business, shipping delightful products and
                    accelerating product and career growth.
                </div>
                <div class="flex flex-col items-end">
                    <div>
                        <img
                            class="duggup-logo"
                            alt="The project logo"
                            src={duggup}
                        />
                    </div>
                    <div class="text-base font-bold">Duggup</div>
                    <div class="text-xs font-normal designation-ceo">
                        Co-Founder and CEO
                    </div>
                </div>
            </div>
            <div class="flex justify-between p-2 w-full items-center">
                <div>
                    <Button.Root class="rounded" on:click={toggleFollow}>
                        {isFollowed ? "Followed" : "Follow"}
                    </Button.Root>
                </div>
                <div class="flex items-center">
                    <div>My website</div>
                    <img
                        class="linkicon m-2"
                        alt="The project logo"
                        src={linkIco}
                    />
                    <img class="icon ml-5" alt="The project logo" src={Icon} />
                </div>
            </div>
        </div>
    </div>

    <div class="flex flex-col w-3/4 mx-auto py-10">
        <div class="flex">
            <div class="flex align-middle items-center w-28 justify-end">
                Dec 2023
            </div>
            <div class="ml-5 flex flex-col items-center">
                <Separator.Root
                    orientation="vertical"
                    class="seperator data-[orientation=horizontal]:h-px data-[orientation=vertical]:h-2/3 data-[orientation=horizontal]:w-full data-[orientation=vertical]:w-[1px]"
                />
                <!-- <div class="seperator"></div> -->
                <div class="ellipse"></div>
                <Separator.Root
                    orientation="vertical"
                    class="seperator data-[orientation=horizontal]:h-px data-[orientation=vertical]:h-2/3 data-[orientation=horizontal]:w-full data-[orientation=vertical]:w-[1px]"
                />
            </div>
            <div class="flex ml-10">
                <div class="flex flex-col card m-5">
                    <div class="">
                        <img
                            class="card-img"
                            alt="The project logo"
                            src={stevejobs}
                        />
                    </div>
                    <div class="text-sm font-normal w-inherit m-auto mx-5">
                        No amount of technology can convert a bad story into a
                        good story.
                    </div>
                </div>
                <div class="flex flex-col card m-5">
                    <div class="">
                        <img
                            class="card-img"
                            alt="The project logo"
                            src={samaltman}
                        />
                    </div>
                    <div class="text-sm font-normal w-inherit m-auto mx-5">
                        Most people don't have original ideas. Here is how Sam
                        Altman pushes himself to have unpopular ideas.
                    </div>
                </div>
            </div>
        </div>

        <div class="flex">
            <div class="flex flex-col align-middle items-end text-right w-28">
                <div class="flex align-middle w-full justify-end">
                    <img
                        class="duggup-logo"
                        alt="The project logo"
                        src={duggup}
                    />
                </div>
                <div class="text-base font-bold">Duggup</div>
                <div class=" flex items-end">
                    San Francisco Bay Area <br />Joined <br /> Nov 2023
                </div>
            </div>
            <div class="ml-5 flex flex-col items-center">
                <img class="chevron" alt="The project logo" src={chevron} />
                <Separator.Root
                    orientation="vertical"
                    class="seperator data-[orientation=horizontal]:h-px data-[orientation=vertical]:h-2/3 data-[orientation=horizontal]:w-full data-[orientation=vertical]:w-[1px]"
                />
                <!-- <div class="seperator"></div> -->
                <div class="ellipse-large"></div>
                <Separator.Root
                    orientation="vertical"
                    class="seperator data-[orientation=horizontal]:h-px data-[orientation=vertical]:h-2/3 data-[orientation=horizontal]:w-full data-[orientation=vertical]:w-[1px]"
                />
                <!-- <img
                            class="chevron"
                            alt="The project logo"
                            src={chevron}
                        /> -->
            </div>

            <div class="ml-10 my-5">
                <div class="text-xl font-bold job-design p-2">
                    Co-Founder and CEO
                </div>
                <div class="text-xs font-normal job-status px-2">
                    Full-time · Remote
                </div>
            </div>
        </div>

        <div class="flex">
            <div class="flex align-middle items-center w-28 justify-end">
                Dec 2023
            </div>
            <div class="ml-5 flex flex-col items-center">
                <Separator.Root
                    orientation="vertical"
                    class="seperator data-[orientation=horizontal]:h-px data-[orientation=vertical]:h-2/3 data-[orientation=horizontal]:w-full data-[orientation=vertical]:w-[1px]"
                />
                <!-- <div class="seperator"></div> -->
                <div class="ellipse"></div>
                <Separator.Root
                    orientation="vertical"
                    class="seperator data-[orientation=horizontal]:h-px data-[orientation=vertical]:h-2/3 data-[orientation=horizontal]:w-full data-[orientation=vertical]:w-[1px]"
                />
            </div>
            <div class="flex ml-10">
                <div class="flex flex-col card m-5">
                    <div class="">
                        <img
                            class="card-img"
                            alt="The project logo"
                            src={startuplesson}
                        />
                    </div>
                    <div class="text-sm font-normal w-inherit m-auto mx-5">
                        Startup Lesson I am reflecting. Don't build for the
                        "average person".
                    </div>
                </div>
                <div class="flex flex-col card m-5">
                    <div class="">
                        <img
                            class="card-img"
                            alt="The project logo"
                            src={cleanshot}
                        />
                    </div>
                    <div class="text-sm font-normal w-inherit m-auto mx-5">
                        Your biggest regrets at 80 will be acts of omission.
                    </div>
                </div>
            </div>
        </div>

        <div class="flex">
            <div class="flex flex-col align-middle items-end text-right w-28">
                <div class="flex align-middle w-full justify-end">
                    <img
                        class="duggup-logo"
                        alt="The project logo"
                        src={betterup}
                    />
                </div>
                <div class="text-base font-bold">Duggup</div>
                <div class=" flex items-end">
                    San Francisco Bay Area <br />Joined <br /> Sep 2022
                </div>
            </div>
            <div class="ml-5 flex flex-col items-center">
                <img class="chevron" alt="The project logo" src={chevron} />
                <Separator.Root
                    orientation="vertical"
                    class="seperator data-[orientation=horizontal]:h-px data-[orientation=vertical]:h-1/3 data-[orientation=horizontal]:w-full data-[orientation=vertical]:w-[1px]"
                />
                <!-- <div class="seperator"></div> -->
                <div class="ellipse-large"></div>
                <Separator.Root
                    orientation="vertical"
                    class="seperator data-[orientation=horizontal]:h-px data-[orientation=vertical]:h-1/3 data-[orientation=horizontal]:w-full data-[orientation=vertical]:w-[1px]"
                />
            </div>
            <div class="ml-10 my-5">
                <div class="text-xl font-bold job-design p-2">
                    VP Engineering
                </div>
                <div class="text-xs font-normal job-status px-2">Full-time</div>
            </div>
        </div>
    </div>
</div>

<style>
    .intro-top {
        color: #4b5c6d;
    }
    .intro-top img {
        width: 120px;
        height: 120px;
        border-radius: 120px;
        border: 5px solid #eaeff5;
    }
    .designation-ceo {
        color: rgba(122, 146, 153, 1);
    }
    .duggup-logo {
        width: 36px;
        height: 36px;
        border-radius: 90px;
    }
    .icon {
        width: 22.4px;
        height: 5.6px;
    }
    .linkicon {
        width: 16px;
        height: 16px;
    }
    .card {
        height: 226px;
        width: 344px;
        border: 0.5px solid rgba(208, 213, 221, 1);
        background: rgba(255, 255, 255, 1);
        border-radius: 12px;
    }
    .card-img {
        width: 344px;
        height: 136px;
        border-top-left-radius: 12px;
        border-top-right-radius: 12px;
        object-fit: cover;
    }
    .job-design {
        color: rgba(20, 22, 24, 1);
    }
    .job-status {
        color: rgba(122, 146, 153, 1);
    }
    .ellipse {
        width: 14px;
        height: 14px;
        border-radius: 16px;
        border: 3px solid rgba(0, 102, 255, 1);
    }
    .ellipse-large {
        width: 16px;
        height: 16px;
        border-radius: 8px;
        border: 5px solid rgba(0, 102, 255, 1);
        box-shadow: 0px 1px 1px 0px rgba(165, 185, 211, 1);
        background: rgba(255, 255, 255, 1);
    }
    .chevron {
        width: 13px;
        height: 6px;
    }
    .nav-chevron {
        width: 13px;
        height: 6px;
        transform: rotate(180deg);
    }
    .nav-icons {
        width: 24px;
        height: 24px;
        padding: 4px;
    }
    .nav-icon-text {
        color: rgba(77, 77, 77, 1);
    }
    .nav-ceo {
        height: 48px;
        width: 48px;
        border-radius: 1000px;
    }
    .navbar{
        border-bottom: 1px solid rgb(154, 154, 155);
    }
</style>
